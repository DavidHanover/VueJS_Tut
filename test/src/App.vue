<template>
  <div id="app">
    <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from './components/Todos.vue'

export default {
  name: 'app',
  components: {
    Todos

  },
  data(){
    return{
      todos: [
        {
          id:1,
          title:"Cut grass",
          completed:false
        },
        {
          id:2,
          title:"Go to store",
          completed:true
        },
        {
          id:3,
          title:"Get hair-cut",
          completed:false
        },
        {
          id:4,
          title:"Clean house",
          completed:false
        }
      ]
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
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
