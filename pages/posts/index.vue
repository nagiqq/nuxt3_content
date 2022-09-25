<template>
<div>
  <h1>blog post--museum</h1>
  <ContentList v-slot="{ list }">
    <div v-for="posts in list" :key="posts._path">
    <h2>{{ posts.name }} </h2>
      <h3>{{ posts.date }}</h3>
      <img :src="posts.img">
      <h3>{{ posts.description }}</h3>
      <div> <a :href="posts._path">閱讀更多→</a></div>
      <hr/>
    </div>
  </ContentList>
</div>
</template>

<script>
export default {
  name: "index"
}
</script>

<style scoped>
img {
  display: block;
}
h1 {
  background: #f1b0b7;
  padding:10px;
}
</style>
