<template>
  <Navbar />
  <footer />
  <Home />
  <About />
  <Blog1 />
  <Blog2 />
  <Blog3 />
  <Blog4 />
  <Register />
  <Login />
  <BlogDetails />
  <CreateBlog />
  <UserDetails />
  <Contact />
</template>
<script>
import Navbar from "./components/Navbar.vue";
import footer from "./components/footer.vue";
import Home from "./components/Home.vue";
import About from "./components/About.vue";
import Blog1 from "./components/Blog1.vue";
import Blog2 from "./components/Blog2.vue";
import Blog3 from "./components/Blog3.vue";
import Blog4 from "./components/Blog4.vue";
import Register from "./components/Register.vue";
import Login from "./components/Login.vue";
import BlogDetails from "./components/BlogDetails.vue";
import CreateBlog from "./components/CreateBlog.vue";
import UserDetails from "./components/UserDetails.vue";
import Contact from "./components/Contact.vue";

export default {
  name: "App",
  components: {
    Navbar,
    footer,
    Home,
    About,
    Blog1,
    Blog2,
    Blog3,
    Blog4,
    Register,
    Login,
    BlogDetails,
    CreateBlog,
    UserDetails,
    Contact,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@200;300;400;500;600;700;800;900&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Nunito", sans-serif;
}
a {
  text-decoration: none;
  color: #2c3e50;
}

main {
  background: #f5f5f5;
  min-height: 100vh;
  /* padding-top: 100px; */
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
