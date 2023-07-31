<!-- Создать компонент UserList, который будет отображать список пользователей из переданного массива. Каждый пользователь должен быть представлен в виде отдельного компонента User, принимающего пропсы с данными о пользователе (например, имя, фамилия, эл. почта) -->
<template>
    <div>
        <p>{{ user.userName }}</p>
        <p>{{ user.lastName }}</p>
        <p>{{ user.email }}</p>
    </div>
</template>

<script>

export default {

    name: 'User',
    props: { user: Object },
};
</script>
