<!-- Разработка приложения для отображения информации о книгах
Требуется создать компонент "Книга" (Book), который будет отображать информацию о книге, такую как название, автор и год издания. Компонент "Книга" должен иметь возможность отображать дополнительные детали о книге по требованию пользователя. Также необходимо создать компонент "Список книг" (BookList), который будет отображать список книг из переданного массива. -->
<template>
    <div>
        <p>{{ book.title }}</p>
        <p>{{ book.author }}</p>
        <p>{{ book.date }}</p>
        <button @click="moreInfo">{{ yes ? 'Скрыть дополнительную информацию' : 'Дополнительные детали о книге' }}</button>
        <ul v-show="yes">
            <li>{{ book.moreInfo }}</li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'Book',
    props: {
        book: Object,
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