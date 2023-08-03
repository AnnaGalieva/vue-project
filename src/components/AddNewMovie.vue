<template>
    <div>
        <input v-model="title" type="text" placeholder="title">
        <input v-model="producer" type="text" placeholder="producer">
        <input v-model="date" type="text" placeholder="date">
        <input v-model="moreInfo" type="text" placeholder="moreInfo">
        <button @click="addMovie">Добавить</button>
    </div>
</template>

<script>
export default {
    name: 'AddNewMovie',
    emits: ['addNMovie'],
    data() {
        return {
            title: '',
            producer: '',
            date: '',
            moreInfo: '',
        };
    },

    methods: {
        addMovie() {
            const newFilm = {
                title: this.title,
                producer: this.producer,
                date: this.date,
                moreInfo: this.moreInfo
            }
            this.title = '';
            this.producer = '';
            this.date = '';
            this.moreInfo = '';
            this.$emit('addNMovie', newFilm)
        }
    },
};
</script>

<style lang="scss" scoped></style>