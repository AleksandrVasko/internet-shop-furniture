<template>
    <div 
        class="hero-info" 
        :style="{backgroundColor: background}">
        <div 
        class="hero-info-text">
            <h2 
                class="hero-info__title"
                :style="{color: colorTitle}">{{title}}</h2>
            <span 
                class="hero-info__description"
                :style="{color: colorDescription}">{{description}}</span>
        </div>
        <ui-button>
            View collection
        </ui-button>
<!--         <a 
            href="#" 
            class="hero-info-link"
            :style="{color: colorLink}">View collection</a> -->
    </div>
    
</template>


<script setup>
import uiButton from '@/components/UI/Button.vue';

const props = defineProps ({
    title: {
        type: String,
        required: false
    },
    description: {
        type: String,
        required: false
    },
    link: {
        type: String,
        required: false
    },
    colorTitle: {
        type: String,
        default: ''
    },
    colorDescription: {
        type: String,
        default: '#726e8d'
    },
    colorLink: {
        type: String,
        default: '#2A254B'
    },
    background: {
        type: String,
        default: '#fff'
    }
});
</script>




<style lang="scss" scoped>
.hero {
    &-info {
        background: #fff;
        max-width: 630px;
        padding: 50px 55px;
        max-height: 444px;
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
    }
}
</style>