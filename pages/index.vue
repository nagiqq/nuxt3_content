<template>
<div>
  <h1>Hello this is index page.<br/>Please press link to pages that introduce how to use content page in nuxt3</h1>
  <NuxtLink to="/blog">to Blog</NuxtLink>
</div>
</template>

<script>
export default {
  name: "index"
}
</script>

<style scoped>
a {
  font-size: 28px;
  background: #f1b0b7;
  color: #0b2e13;
  text-decoration:  none;
  padding: 10px;
}
</style>
