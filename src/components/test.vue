<template>
  <div class="blog-post">
    <h3>{{ post.title }}</h3>
    <button v-on:click="$emit('enlarge-text')">
      放大文本
    </button>
    <div v-html="post.content"></div>
  </div>
</template>

<script>
export default {
  name: 'test',
  props: ['post']
}
</script>

<style scoped>

</style>
