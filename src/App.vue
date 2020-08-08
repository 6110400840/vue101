<template>
  <div id="app">
    <img src="./assets/logo.png" />
    <h1 :title="msg">{{ msg }}</h1>
    
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-view></router-view>
  </div>
</template>

<script>
import Counter from './Counter.vue'
export default {
  name: "app",
  data() {
    return {
      msg: "Vue101 on CS443",
      number: 0,
      url: 'https://google.com',
      isShow: false
    }
  },
  components : {
    Counter
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
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
</style>
