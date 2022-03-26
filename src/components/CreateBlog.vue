<template>
  <section id="createblog">
    <br />
    <br />
    <form @submit.prevent="createBlog" class="form neu-border">
      <h2 class="form-heading">Create a blog</h2>
      <input
        class="form-input neu-border-inset"
        type="text"
        v-model="title"
        placeholder="Title"
        required
      />
      <input
        class="form-input neu-border-inset"
        type="text"
        v-model="image"
        placeholder="Image"
        required
      />
      <textarea
        class="form-input neu-border-inset"
        type="text"
        v-model="body"
        placeholder="Body"
        required
      ></textarea>

      <button type="submit" class="form-btn neu-border">Create Blog</button>
    </form>
  </section>
</template>

<script>
export default {
  data() {
    return {
      title: "",
      body: "",
      image: "",
    };
  },
  methods: {
    createBlog() {
      // if (!localStorage.getItem("jwt")) {
      //   alert("User not logged in");
      //   // return this.$router.push({ name: "Login" });
      // }
      fetch("https://capstone-backend-a.herokuapp.com/users", {
        method: "POST",
        body: JSON.stringify({
          title: this.title,
          body: this.body,
          img: this.img,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
          Authorization: `Bearer ${localStorage.getItem("jwt")}`,
        },
      })
        .then((response) => response.json())
        .then((json) => {
          alert("Blog Created");
          // this.$router.push({ name: "Blogs" });
        })
        .catch((err) => {
          alert(err);
        });
    },
  },
};
</script>

<style scoped>
#createblog {
  min-height: 100vh;
  padding-top: 120px;
}
.neu-border {
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
  height: 500px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 40px;
  gap: 20px;
  width: 100%;
  max-width: 600px;
  margin: auto;
}

.form-heading {
  text-align: center;
  text-transform: uppercase;
}

.form-input,
.form-btn {
  border: none;
  outline: none;
  padding: 20px;
  height: 500px;
}

.form-btn {
  cursor: pointer;
  transition: all 0.1s linear;
}

.form-btn:hover {
  transform: scale(1.05);
}
</style>
