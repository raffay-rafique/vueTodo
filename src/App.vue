<template>
  <div id="app">
    <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>

import Todos from './components/Todos';


export default {
  name: 'App',
  components: {
    Todos
    
  },
  data(){
    return{
      todos:[{
        id:1,
        title:"Todo One",
        completed:false
      },
      {
        id:2,
        title:"Todo 2",
        completed:false
      },
      {
        id:3,
        title:"Todo 3",
        completed:false
      }]
    }
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  line-height: 1.4;
}
</style>
