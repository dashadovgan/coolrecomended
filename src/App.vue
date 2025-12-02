<template>
  <div id="app"> <!-- Корневой элемент -->
    <NavigationBar />
    <HomePage />
  </div>
</template>

<script>
import NavigationBar from './components/NavigationBar.vue';
import HomePage from './views/HomePage.vue';

export default {
  name: 'App',
  components: {
    NavigationBar,
    HomePage
  }
};
</script>

<style>
/* глобальные стили можно здесь */
body {
  margin: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
