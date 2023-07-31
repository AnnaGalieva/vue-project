<!-- Создать компонент UserList, который будет отображать список пользователей из переданного массива. Каждый пользователь должен быть представлен в виде отдельного компонента User, принимающего пропсы с данными о пользователе (например, имя, фамилия, эл. почта) -->
<template>
    <User :user="user" v-for="user in userList" :key="user.id" />
    <div>

    </div>
</template>

<script>
import User from './User.vue';
export default {

    name: 'UserList',
    components: { User },
    data() {
        return {
            userList: [{
                userName: 'Aaa',
                lastName: 'Bbb',
                email: 'tttt@mail.ru'
            }, {
                userName: 'Rrr',
                lastName: 'Fff',
                email: 'tttt@mail.ru'
            }, {
                userName: 'Yyy',
                lastName: 'Nnn',
                email: 'tttt@mail.ru'
            },]
        };
    },


};
</script>
