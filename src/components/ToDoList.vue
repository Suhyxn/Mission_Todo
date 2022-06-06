<template>
  <div id="todolist">
    <div
      v-for="data in todos"
      id="container"
      :key="data.id">
      <li id="text">
        {{ data }}
      </li>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    todos: []
  }
}
</script>

<style></style>
