<template>
  <section id="about">
    <h1><b>Welcome to Feel Good Foodie</b></h1>
    <br />
    <p>
      Feel Good Foodie is a blog, producing stylish and elegant home-made
      recipes using farm fresh ingredients. Each recipe has been carefully hand
      crafted. Uniquely and importantly, we use fresh garden ingredients - which
      locks in all the goodness and flavour. Scroll down to see more... Our
      recipes comes with simple cooking instructions We guarantee our recipes
      will not fail to impress, and you will feel proud to serve Feel Good
      Foodie meals to anyone sitting at your table.
    </p>
    <br />
    <h2>Take a look at our Favourite dishes</h2>
    <br />

    <div class="container">
      <div class="row">
        <!-- card 1 -->
        <div class="col-md-3">
          <div class="content">
            <a href="#">
              <div class="content-overlay"></div>
              <img
                class="content-image"
                src="https://www.thelastfoodblog.com/wp-content/uploads/2021/11/lentil-cottage-pie-new-f_i.jpg"
              />
              <div class="content-details fadeIn-bottom">
                <h3 class="content-title">Beef cottage pie</h3>
                <div class="btn" @click="goToBlog1()">
                  <a href="#blog1" class="btn"><b>more ...</b></a>
                </div>
              </div>
            </a>
          </div>
        </div>
        <!-- card 2 -->
        <div class="col-md-3">
          <div class="content">
            <a href="#">
              <div class="content-overlay"></div>
              <img
                class="content-image"
                src="https://cdn.shopify.com/s/files/1/0355/9974/5157/products/MG_0379_700x.jpg?v=1584968401"
              />
              <div class="content-details fadeIn-bottom">
                <h3 class="content-title">Apple and Raspberry Crumble</h3>
                <div class="btn" @click="goToBlogs2()">
                  <a href="#blog2" class="btn"><b>more ...</b></a>
                </div>
              </div>
            </a>
          </div>
        </div>
        <!-- card 3 -->
        <div class="col-md-3">
          <div class="content">
            <a href="#">
              <div class="content-overlay"></div>
              <img
                class="content-image"
                src="https://cdn.shopify.com/s/files/1/0355/9974/5157/products/MG_0319copy_700x.jpg?v=1585657843"
              />
              <div class="content-details fadeIn-bottom">
                <h3 class="content-title">Butter chicken</h3>

                <div class="btn" @click="goToBlog3()">
                  <a href="#blog3" class="btn"><b>more ...</b></a>
                </div>
              </div>
            </a>
          </div>
        </div>
        <!-- card 3 -->
        <div class="col-md-3">
          <div class="content">
            <a href="#">
              <div class="content-overlay"></div>
              <img
                class="content-image"
                src="https://cdn.shopify.com/s/files/1/0355/9974/5157/products/GOODNESSGRACIOUSDAY211443_700x.jpg?v=1626774829"
              />
              <div class="content-details fadeIn-bottom">
                <h3 class="content-title">
                  Cauliflower cheese with honey bacon
                </h3>
                <div class="btn" @click="goToBlog4()">
                  <a href="#blog4" class="btn"><b>more ...</b></a>
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    goToBlog1() {
      this.$router.push("/blog1");
    },
    goToBlog2() {
      this.$router.push("/blog2");
    },
    goToBlog3() {
      this.$router.push("/blog3");
    },
    goToBlog4() {
      this.$router.push("/blog4");
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Roboto");

/* .card {
  display: inline-block;
  margin-left: 5px;
  margin-right: 5px;
}
.card-body {
  padding: none;
  margin: none;
}
.card-text {
  height: 40px;
  font-size: 15px;
  padding: none;
  margin: none;
} */

/* .container {
    margin-top: 200px;
    display: inline-block;
} */
.btn {
  background-color: white;
  border-radius: 30px;
}
.title {
  color: #1a1a1a;
  text-align: center;
  margin-bottom: 10px;
}

.content {
  display: flex;
  position: relative;
  width: 100%;
  max-width: 400px;
  margin: none;
  padding: none;
  overflow: hidden;
}

.content .content-overlay {
  background: rgba(0, 0, 0, 0.7);
  position: absolute;
  height: 100%;
  width: 100%;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content:hover .content-overlay {
  opacity: 1;
}

.content-image {
  width: 100%;
  height: 100%;
  border-radius: 30px;
}

img {
  box-shadow: 1px 1px 5px 1px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details {
  top: 50%;
  left: 50%;
  opacity: 1;
}

.content-details h3 {
  color: #fff;
  font-weight: 500;
  letter-spacing: 0.15em;
  margin-bottom: 0.5em;
  text-transform: uppercase;
}

.content-details p {
  color: #fff;
  font-size: 0.8em;
}

.fadeIn-bottom {
  top: 80%;
}

h1 {
  margin-top: 30px;
}

h2 {
  font-size: 2rem;
}

p {
  position: relative;
  padding-left: 100px;
  padding-right: 100px;
  font-size: 25px;
}
#about {
  z-index: 1;
  padding-top: 120px;
  min-height: 100vh;
}
</style>
