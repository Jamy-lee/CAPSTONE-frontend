<template>
  <section id="blog3">
    <!-- card 1 -->

    <h2>Butter chicken</h2>
    <br />
    <div class="row">
      <div class="col-md-6">
        <img
          class="content-image"
          src="https://cdn.shopify.com/s/files/1/0355/9974/5157/products/MG_0319copy_700x.jpg?v=1585657843"
        />

        <br />
      </div>
      <div class="col-md-6">
        <h3>Ingredients</h3>
        <p></p>
        <pre>
    1 tablespoon oil
    1 tablespoon butter
    1 medium onion diced
    1 teaspoon fresh ginger finely minced or grated (or use paste)
    2-3 cloves garlic finely minced or crushed
    1 ½ pounds about 2-3 boneless, skinless chicken breasts, cut into ¾-inch chunks
    4 tablespoons tomato paste or 8 oz can of tomato sauce
    1 tablespoon garam masala
    1 teaspoon  or paprika, adjust to taste
    1 teaspoon Fenugreek I use powder, but seeds or mustard seeds can be used too, optional*
    1 teaspoon cumin
    1 tsp salt
    1/4 tsp black pepper
    1 cup heavy cream sub for half and half or yogurt for low fat
    Hot cooked rice and naan for serve
          </pre
        >
        <h3>Instructions</h3>
        <ol>
          <li>
            Heat a large skillet or medium saucepan over medium-high heat. Add
            the oil, butter, and onions and cook onions down until lightly
            golden, about 3-4 minutes. Add ginger and garlic and let cook for 30
            seconds, stirring so it doesn’t burn.
          </li>
          <li>
            Add the chicken, tomato paste, and spices. Cook for 5-6 minutes or
            until everything is cooked through.
          </li>
          <li>
            Add the heavy cream and simmer for 8-10 minutes stirring
            occasionally. Serve over Basmati rice or with naan.
          </li>
        </ol>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#blog3 {
  min-height: 100vh;
  padding-top: 120px;
}
h2 {
  position: relative;
  padding-top: 12px;
}
.content-image {
  height: 50%;
  border: white solid 10px;
  border-radius: 30px;
  box-shadow: 8px 8px 15px #e4e4e4, -8px -8px 15px #ffffff;
}
h3 {
  color: #cf332c;
}
li {
  /* margin-right:10px; */
  padding: 5px;
  text-align: left;
}
pre {
  margin-right: 10px;
  padding: 5px;
  font-size: 15px;
  font-family: "Nunito", sans-serif;
  text-align: left;
  color: #2c3e50;
}
p {
  font-size: 20px;
}
</style>
