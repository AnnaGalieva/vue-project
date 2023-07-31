<template>
    <h1>{{ text }},
        Привет из компонента hello
    </h1>
</template>
<script>
export default {
    props:{
        text:String,
    },
    name: 'hello',
};
</script>
<style scoped lang="scss">
h1{color: red;}
</style>