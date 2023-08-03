<template>
  <!-- <h1>Привет из APP vue</h1> -->
  <!-- <Hello :text="text" />
<Gallery /> -->
  <!-- <Authentication: isAuth="isAuthenticated" /> -->
  <!-- //передали пропс -->
  <!-- <UserList />
  <MortgageCalculator /> -->
  <BookList />
  <MovieList />
</template>

<script>
import BookList from './components/BookList.vue';
import MovieList from './components/MovieList.vue';

// import Hello from './components/Hello.vue';
// import Gallery from './components/Gallery.vue';
// import Authentication from './components/Authentication.vue'
// import UserList from './components/UserList.vue';
// import MortgageCalculator from './components/MortgageCalculator.vue';


export default {

  name: 'App',
  components: {
    BookList,
    MovieList
  },

  data() {
    return {
      // text: 'kkkkkkkk',
      // isAuthenticated: false,
    };
  },
}
</script>

<style lang="scss"></style>
<!-- <template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style> -->

