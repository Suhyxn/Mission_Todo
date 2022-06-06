<template>
  <img
    src="./assets/logo.png"
    alt="Vue logo" />
  <to-do-head name="TO-DO" />
  <to-do-input @add-to-do="addToDo" />
  <to-do-list
    :todos="todos" />
</template>

<script> 
import ToDoHead from './components/ToDoHead.vue'
import ToDoInput from './components/ToDoInput.vue'
import ToDoList from './components/ToDoList.vue'

export default {
  name: 'App',
  components: {
    ToDoHead,
    ToDoInput,
    ToDoList
  },
  data() {
    return {
      todos: ['발 닦기']
    }
  },
  methods: {
    addToDo(content) {
      this.todos.push(content)
    }
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
