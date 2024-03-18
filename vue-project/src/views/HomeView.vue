<template>
  <div>
    <h1>Make a Poke Bowl!</h1>
    <IngredientCard v-for="ingredient in ingredients" :key="ingredients.name":ingredient="ingredient"/>
  </div>
  <div>
    <ItemCart :cart="cart"/>
  </div>
</template>

<script setup>
import IngredientCard from '@/components/IngredientCard.vue';
import ItemCart from '@/components/ItemCart.vue';
const ingredients = [
  {
    name: "Sushi Rice",
    price: "0.50",
    category: "base",
    image:"https://freepngimg.com/thumb/rice/35748-3-rice-transparent.png"
  },
  {
    name: "Soba",
    price: "0.50",
    catgory: "base",
    image: "https://static.vecteezy.com/system/resources/previews/026/774/090/non_2x/soba-with-ai-generated-free-png.png",
  },
  {
    name: "Brown Rice",
    price: "0.50",
    catgory: "base",
    image: "    image: https://www.bluemountainorganics.com/pub/media/catalog/product/cache/443d0ed8cb3817b2d3cb38abd802d77f/l/g/lgbr.png",
  },
  {
    name: "Zucchini Noodles",
    price: "0.50",
    catgory: "base",
    image: "https://southfinpoke.com/wp-content/uploads/2018/07/zucchini-noodles.png",
  },
  {
    name: "Salmon",
    price: "0.70",
    catgory: "meat",
    image: "https://assets-global.website-files.com/5b0d8277929f696d703d2e87/64a82ef09387f7c9e5817960_salmon-hero.png",
  },
  {
    name: "Ahi Tuna",
    price: "0.70",
    catgory: "meat",
    image: "https://www.blueworldseafood.com/wp-content/uploads/2021/12/121149-092-e1641475629234.png",
  },
  {
    name: "Shrimp",
    price: "0.70",
    catgory: "meat",
    image: "https://pngimg.com/d/shrimps_PNG18278.png",
  },
  {
    name: "Chicken",
    price: "0.70",
    catgory: "meat",
    image: "https://barberitos.com/wp-content/uploads/2017/08/Menu-Chicken.png",
  },
  {
    name: "Sweet Corn",
    price: "0.50",
    catgory: "add-ins",
    image: "https://gallery.yopriceville.com/var/resizes/Free-Clipart-Pictures/Vegetables-PNG/Sweet_Corn_Grains_PNG_Clip_Art_Image.png?m=1534117454",
  },
  {
    name: "Cilantro",
    price: "0.50",
    catgory: "add-ins",
    image: "https://fruitbubba.com/wp-content/uploads/2022/05/usa-bubba-fruit-parsley-1.png",
  },
  {
    name: "Cucumbers",
    price: "0.50",
    catgory: "add-ins",
    image: "https://gallery.yopriceville.com/var/resizes/Free-Clipart-Pictures/Vegetables-PNG/Sliced_Cucumber_Transparent_PNG_Clip_Art_Image.png?m=1529142599",
  },
  {
    name: "Seaweed Salad",
    price: "0.50",
    catgory: "add-ins",
    image: "https://ocoee.toukensushi.com/cdn/shop/products/SEAWEEDSALAD_b3b5cd93-aac8-4088-b7f0-c8c5547e3ed1.png?v=1603319632",
  },
  {
    name: "Masago",
    price: "0.50",
    catgory: "add-ins",
    image: "https://azumafoods.com/wp/wp-content/uploads/2021/01/82716-Masago-Hybrid.png",
  },
  {
    name: "Chopped Mango",
    price: "0.50",
    catgory: "add-ins",
    image: "https://static.wixstatic.com/media/636a8e_aaa3888e59b648459d151f8fa8f354cb~mv2.png/v1/fill/w_552,h_440,al_c,lg_1,q_85,enc_auto/mango.png",
  },
  {
    name: "Cherry Tomato",
    price: "0.50",
    catgory: "add-ins",
    image: "https://www.lipmanfamilyfarms.com/wp-content/uploads/2020/09/CherryTomato-hero@2x-1024x704.png",
  },
  {
    name: "Avocado",
    price: "0.50",
    catgory: "add-ins",
    image: "https://www.schlotzskys.com/-/media/schlotzskys/ingredients/dicedavocado-400.png?v=1&d=20180213T143540Z",
  },
  {
    name: "Wonton Crisps",
    price: "0.50",
    catgory: "add-ins",
    image: "https://www.wontonfood.com/media_files/images/4117f9982c82e06bd03c41a167878bb3.max-1900x1900.png",
  },
  {
    name: "Nori",
    price: "0.50",
    catgory: "add-ins",
    image: "https://foodconnection-shop.de/WebRoot/Store28/Shops/41cdaff9-d12c-4380-8bb5-14183a0ad0af/55FE/FC6F/AE51/8F21/C119/0A48/3572/726A/sushi_algen_premium_jp1044_ml.png",
  },
]


</script>

<style scoped>

</style>