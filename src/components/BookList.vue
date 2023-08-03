<template>
    <div>
        <Book :book="book" v-for="book in books" :key="book.id" />
    </div>
</template>

<script>
import Book from './Book.vue'
export default {
    name: 'BookList',
    components: {
        Book
    },

    data() {
        return {
            books: [{
                title: 'Книга 1',
                author: 'Автор 1',
                date: 2020,
                moreInfo: 'aaa'
            }, {
                title: 'Книга 2',
                author: 'Автор 2',
                date: 2019,
                moreInfo: 'aaa'
            }, {
                title: 'Книга 3',
                author: 'Автор 3',
                date: 2021,
                moreInfo: 'aaa'
            }, {
                title: 'Книга 4',
                author: 'Автор 4',
                date: 2022,
                moreInfo: 'aaa'
            },]
        };
    },

    methods: {

    },
};
</script>

<style lang="scss" scoped></style>