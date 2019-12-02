<template>
  <section>
    <ul v-for="post in blogPosts" :key="post.id">
      <li>
        {{ post.title }}
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  computed: {
    blogPosts () {
      return this.$store.state.blogPosts;
    },
  },
};
</script>

<style>

</style>
