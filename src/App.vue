<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/classic-food-pic.jpg">
    <NinerReviewsPage/>
  </div>
</template>

<script>
import NinerReviewsPage from './components/pages/NinerReviewsPage';

export default {
  name: 'app',
  components: {
    NinerReviewsPage
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
