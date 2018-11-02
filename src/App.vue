<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Proxima+Nova');

html, body {
  font-family: 'Proxima Nova', sans-serif;
}

body {
  font-family: 'Proxima Nova', sans-serif;
}


#app {
  font-family: 'Proxima Nova', 'Avenir',sans-serif;
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.logo{
  width: 109px;
}

.logo a{
  color: #40b75f;
}

a:hover{
  color: #40b75f !important;
}
a{
  text-decoration:none;
}
a:hover{
  text-decoration: none;
}
</style>
