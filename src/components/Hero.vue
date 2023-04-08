<template>
    <div class="hero">     
        <HeroInformation 
        title="Luxury homeware for people who love timeless design quality"
        description="With our new collection, view over 400 bespoke pieces from homeware through to furniture today"
        link="#"/>        
    </div>
</template>


<script setup>
import HeroInformation from '@/components/HeroInformation.vue';
</script>


<style lang="scss" scoped>
.hero {
    background: url('/public/img/Hero Blocks.jpg');
    height: 704px;
    margin: 0 22px;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding-right: 80px;
    &-img {
        max-width: 100%;
    }
    /* &-info {
        background: #fff;
        max-width: 630px;
        padding: 50px 55px;
        height: 444px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        &__title {
            font-family: 'Clash-Display', sans-serif;
            font-weight: 400;
            line-height: 1.5;
            margin: 0 0 20px 0;
        }
        &__description {
            color: #5b5676;
            font-size: 18px;
        }
        &-link {
            color: #2A254B;
            text-decoration: none;
                &:hover {
                text-decoration: underline;
            }
        }
    } */
}
</style>