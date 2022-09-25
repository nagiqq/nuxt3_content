<template>
<div>
  <ContentDoc v-slot="{ doc }">
    <div>Collection in {{ doc.name }}</div>
    <hr/>
      <div v-for="colletion in doc.collections">
    <img :src="colletion.img">
    <h3>{{ colletion.name }}</h3><hr/>
    </div>
    <ContentRenderer :value="doc"/>
  </ContentDoc>
</div>
</template>

<script>
export default {
  name: "[slut]"
}
</script>

<style scoped>
img {
  max-width: 150px;
}
</style>
