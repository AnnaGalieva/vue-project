<!-- Создайте компонент "Аутентификация" (Authentication), который будет отображать форму входа или сообщение об успешной аутентификации в зависимости от переданного пропса isAuthenticated. Используйте директиву v-if для условного отображения разных элементов в шаблоне компонента. -->
<template>
    <div>
        <p v-if="isAuth">вошли в систему</p>
        <form v-else>
            Логин<input type="text" /><br />
            Пароль<input type="text" /><br />
            <button>Войти</button>
        </form>
    </div>
</template>

<script>
export default {
    props: { isAuth: Boolean },
    name: 'Authentication',


    data() {
        return {

        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>

<style lang="scss" scoped></style>