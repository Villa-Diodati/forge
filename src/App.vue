<template>
  <div id="app">
    <Navigation />
    <router-view></router-view>
  </div>
</template>

<script>
import Navigation from './components/navigation.vue'

export default {
  name: 'app',
  components: {
    Navigation,
  },
}
</script>

<style lang='scss'>
@import './constants/scss-variables.scss';

html, body, #app {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Raleway', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $forgeGrey;
}

ul {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

</style>
