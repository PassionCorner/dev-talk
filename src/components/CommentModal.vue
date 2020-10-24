<template>
  <div class="c-container">
    <a @click="$emit('close')">close</a>
    <p>add a comment</p>
    <form @submit.prevent>
      <textarea v-model.trim="comment"></textarea>
      <button @click="addComment()" :disabled="comment == ''" class="button">add comment</button>
    </form>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
