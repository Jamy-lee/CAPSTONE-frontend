<template>
  <section id="contact">
    <h1><b>Contact us</b></h1>
    <br />
    <form
      action="https://formspree.io/f/meqnlowj"
      method="POST"
      class="form neu-border"
      target="_blank"
    >
      <input
        required
        class="form-input neu-border-inset"
        type="name"
        name="name"
        v-model="text"
        placeholder="Names"
      />
      <input
        required
        class="form-input neu-border-inset"
        type="email"
        name="email"
        v-model="email"
        placeholder="Email"
      />
      <input
        required
        class="form-input neu-border-inset"
        type="number"
        name="number"
        v-model="number"
        placeholder="Contact number"
      />
      <div class="button">
        <button type="submit" class="form-btn neu-border">Submit</button>
        <button type="reset" class="form-btn neu-border">Reset</button>
      </div>
    </form>
  </section>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "",
      email: "",
      number: "",
      message: "",
    };
  },
  methods: {
    handleSubmit() {
      console.log(this.name, this.email, this.contact, this.message);
      fetch("...", {
        method: "POST",
        body: JSON.stringify({
          name: this.name,
          email: this.email,
          number: this.number,
          message: this.message,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => {
          console.log(json);
          alert("Message sent successfully");
          (this.name = ""),
            (this.email = ""),
            (this.number = ""),
            (this.message = "");
        });
    },
  },
};
</script>

<style>
#contact {
  height: 100vh;
  padding-top: 120px;
}
input {
  height: 350px;
  border: none;
  border-radius: 30px;

  box-shadow: inset 8px 8px 15px #e4e4e4, inset -8px -8px 15px #ffffff;
}

h1 {
  margin-top: 30px;
}

.neu-border {
  height: 500px;
  border-radius: 30px;
  background: #f5f5f5;
  box-shadow: 8px 8px 15px #e4e4e4, -8px -8px 15px #ffffff;
}
.neu-border-inset {
  border-radius: 30px;
  background: #f5f5f5;
  box-shadow: inset 8px 8px 15px #e4e4e4, inset -8px -8px 15px #ffffff;
}

.form {
  margin: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 40px;
  gap: 20px;
  width: 100%;
  margin: auto;
  max-width: 600px;
}

.form-heading {
  text-align: center;
  text-transform: uppercase;
}

.form-input,
.form-btn {
  height: 70px;
  border: none;
  outline: none;
  padding: 20px;
  margin-right: 10px;
}

.form-btn {
  height: 60px;
  margin-left: 5px;
  width: 150px;
  cursor: pointer;
  transition: all 0.1s linear;
}

.form-btn:hover {
  transform: scale(1.05);
}
</style>
