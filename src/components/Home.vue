<template>
  <section id="home">
    <h1>Feel Good Foodie</h1>

    <p>Food is not about impressing people.</p>

    <p>It’s about making them feel comfortable.</p>
    <!-- register button -->
    <div id="button" @click="goToLogin()">
      <a href="#login" class="btn btn-danger"><b>Login here</b></a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#home {
  height: 100vh;
  background: url(https://images.unsplash.com/photo-1455619452474-d2be8b1e70cd?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80);
  /* opacity: 80%; */
  /* background-color: black; */
  background-size: 100%;
  background-repeat: no-repeat;
  background-attachment: fixed;
  /* z-index:1; */
}

.btn-danger {
  height: 80px;
  width: 200px;
  text-align: center;
  padding-top: 20px;
  position: relative;
  font-size: 25px;
  top: 300px;
  right: 500px;
  border-radius: 60px;
  box-shadow: 5px 5px 15px #0e0d0d, -5px -5px 15px #0e0d0d;
}
p {
  color: white;
  text-shadow: 0 1px 0;
  position: relative;
  top:180px;
  right: 450px;
  font-size: 30px;
}
h1 {
  margin-right: 55%;
  color: white;
  /* z-index: -; */
  font-size: 4.5em;
  position: relative;
  padding-top: 130px;
  text-shadow: 2px 2px 5px black;
  /* margin-top: 100px; */
  background-attachment: relative;
}

/* #button {
  position: relative;
  top: 200px;
} */
</style>
