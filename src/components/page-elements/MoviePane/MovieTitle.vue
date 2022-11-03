<template>
  <h1>{{ title }}</h1>
</template>

<script>
export default {
  name: "MovieTitle",
  props: ["title"]
}
</script>

<style scoped>
div {
  border: solid 1px darkcyan;
}
</style>