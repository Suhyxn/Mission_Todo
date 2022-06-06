<template>
  <div id="todoinput">
    <input
      v-model="content"
      type="text" />
    <button
      type="button"
      @click="addToDo">
      제출
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      content: ''
    }
  },
  methods: {
    addToDo() {
      alert('등록하겠습니다.')
      this.$emit('add-to-do', this.content)
      this.content = ''
    }
  }
}
</script>

<style>
</style>
