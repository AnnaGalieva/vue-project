<template>
    <div>
        <p>{{ movie.title }}</p>
        <p>{{ movie.producer }}</p>
        <p>{{ movie.date }}</p>
        <button @click="moreInfo">{{ yes ? 'Скрыть дополнительную информацию' : 'Дополнительные детали о фильме' }}</button>
        <ul v-show="yes">
            <li>{{ movie.moreInfo }}</li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'MovieInfo',
    props: {
        movie: Object,
    },

    data() {
        return {
            yes: false
        };
    },

    methods: {
        moreInfo() {
            this.yes = !this.yes
        }
    },
};
</script>

<style lang="scss" scoped></style>