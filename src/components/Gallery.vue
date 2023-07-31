<template>
    <h1>
        Привет из Gallery
    </h1>
    <img :src="src" alt="pic">
    <div><img @click="changeImage(image.src)"  v-for="image in images" :key="image.id" :src="image.src" alt="pic"></div>
    <!-- <div class="gallery"><img :src="currentImage" alt="Большое изображение"></div>
    <div><img v-for="(image,index) in images" :key="index" :src="image" @click="changeImage"></div> -->
</template>
<script>
export default {
    name: 'Gallery',
    data() {
        return {
            src:'',
            images: [
                {src:require("@/assets/img/product1.svg")},
                {src:require("@/assets/img/product2.svg")},
                {src:require("@/assets/img/product3.svg")},
                {src:require("@/assets/img/product4.svg")},

            ],
        }
    },methods: {
        changeImage(src) {
           this.src=src
        },
    },
};
</script>
<style scoped lang="scss">
h1{color: red;}
</style>