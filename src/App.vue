<template>
 <div>
    <MenuComponent/>
    <h1>ELEMENTO ESTATICO</h1>
    <hr/>>
    <!--ESTO ES UN ELEMENTO DINAMICO -->
    <router-view></router-view>
    <hr/>
 </div>
  <!-- <HolaMundo/>>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <MusicaComponent/>
  <CineComponent/>
  <HomeComponent/> -->
</template>

<script>
import MenuComponent from './components/MenuComponent.vue'
// import HelloWorld from './components/HelloWorld.vue'
// import HolaMundo from './components/HolaMundo.vue'
// import HomeComponent from './components/HomeComponent.vue'
// import MusicaComponent from './components/MusicaComponent.vue'
// import CineComponent from './components/CineComponent.vue'
export default {
  name: 'App',
  components: {
    MenuComponent
    // HelloWorld , HolaMundo , MusicaComponent, HomeComponent ,CineComponent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
