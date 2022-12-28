<template>
  <div class="products-container">
    <div class="products">
      <Product 
      v-for="product of products" 
      :key="product.id"
      :img="product.img"
      :title="product.title"
      :price="product.price"/>
   </div>
   <a href="#" class="products-link">View collection</a>
  </div>
   
</template>

<script setup>
import { ref } from 'vue'
import Product from '../components/Product.vue';

const products = ref([
  {
    id: 1,
    img: '/svg/product1.svg',
    title: 'The Dandy chair',
    price: 250
  },
  {
    id: 2,
    img: '/svg/product2.svg',
    title: 'Rustic Vase Set',
    price: 155
  },
  {
    id: 3,
    img: '/svg/product3.svg',
    title: 'The Silky Vase',
    price: 125
  },
  {
    id: 4,
    img: '/svg/product4.svg',
    title: 'The Lucy Lamp',
    price: 399
  }
]);

</script>

<style lang="scss" scoped>
.products {
   padding: 0 80px;
   display: flex;
   grid-template-columns: repeat(4, 1fr);
   column-gap: 20px;
   margin-bottom: 64px;
   &-container {
    margin-bottom: 56px;
   }
   &-link {
    display: block;
    text-align: center;
    color: #2A254B;
    text-decoration: none;
    &:hover {
      text-decoration: underline;
    }
   }
}
</style>