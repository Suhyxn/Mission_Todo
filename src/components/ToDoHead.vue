<template>
  <div id="todohead">
    <h1>{{ name }}</h1>
  </div>
</template>

<script>
export default {
  name: 'ToDoHead',
  props : {
    name: String
  }
}
</script>

<style>
</style>
