<template lang='pug'>
#app
  router-view
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
body {
  width: 100%;
  margin: 0 0;
}
html {
  height: 0;
}
@import url('https://fonts.googleapis.com/css?family=Montserrat');
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
}
</style>
