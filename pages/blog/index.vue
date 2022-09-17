<template>
<div>
  <h1>blog post--museum</h1>
  <ContentList v-slot="{ list }">
    <div v-for="article in list" :key="article._path">
    <h2>{{ article.name }} </h2>
      <h3>{{ article.date }}</h3>
      <img :src="article.img">
      <h3>{{ article.description }}</h3>
      <div> <a :href="article._path">閱讀更多→</a></div>
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
