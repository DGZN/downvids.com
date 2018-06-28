<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
  @import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>

<script>
export default {
  name: 'App'
}
</script>

<style>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
body {
    margin: 0;
    text-align: center;
}
html {
  margin:auto;
      position:relative;
      top:-8px;
      left:-8px;
}

#app {
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  padding: 0px; */
}
</style>
