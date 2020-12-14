<template>
  <div id="app">
     
    <Header/>
    <Content/>
    <Zmija/>
    <Tretji/>
    
  </div>
</template>

<script>
import Content from './components/Content.vue'
import Zmija from './components/Zmija.vue'
import Header from './components/Header.vue'
import Tretji from './components/Tretji.vue'


export default {
  name: 'App',
  components: {
    
    Content,
    Zmija,
    Header,
    Tretji
    
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
  margin-top: 100px;
  
}
.body,html { 
  padding:0;
  margin:0;
  background-color: #f6f5fb;
  min-height: 100%;
}
</style>
