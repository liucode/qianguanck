<template>
    <div id="app">
        <NavBar/>
        <Billboard/>
        <router-view/>
        <Footer></Footer>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Billboard from './components/Billboard'
import Footer from './components/Footer'
export default {
  components: {
    NavBar,
    Billboard,
    Footer
  }
}
</script>

<style>
body {
    margin: 0px;
}
body::-webkit-scrollbar {
    width: 0px;
}
hr {
    background-color: #D0D0D0;
    height: 1px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#NavBar {
    position: fixed;
    z-index: 100000;
    background-color: white;
    width: 100%;
    border-bottom: 1px #D0D0D0 solid;
}
#Billboard {
    padding-top: 50px;
    margin-bottom: 15px;
}
</style>
