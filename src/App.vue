<template>
  <div class="container">
      <Header />
      <Hero />
      <AboutBrand />
      <Products />
      <Ideas />
  </div>
</template>  


<script setup>
import Header from './components/Layout/Header.vue'
import Hero from './components/Hero.vue'
import AboutBrand from './components/AboutBrand.vue'
import Products from './components/Products4Column.vue'
import Ideas from './components/Ideas.vue'
</script>



<style lang="scss">
@import url('http://fonts.cdnfonts.com/css/satoshi');
@import url('http://fonts.cdnfonts.com/css/clash-display');

* {
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

body {
  margin: 0;
  padding: 0;
  font-size: 16px;
  font-family: 'Satoshi', sans-serif;
  //font-family: 'Clash-Display', sans-serif;

}

.container {
  max-width: 1140px;
  margin: 0 auto;
}
</style>
