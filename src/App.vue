<template>
  <div id="app">
    <Todos v-bind: todos="todos"/>
  </div>
  
</template>

<script>
import Todos from './components/Todos';
export default {
  name: "App",
  components: {
    Todos
  },
  data() {
    return{
      todos:[
        {
          id: 1,
          title: "To do One",
          completed: false
          },
          {
            id : 2,
            title:"To do Two",
            completed: true
          },
          {
            id: 3 ,
            title: "To do Three",
            completed: true
          }
      ]
    }
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
