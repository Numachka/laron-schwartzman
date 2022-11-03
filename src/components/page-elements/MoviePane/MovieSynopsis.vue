<template>
<div>{{ synopsis }}</div>
</template>

<script>
export default {
  name: "MovieSynopsis",
  props: ["synopsis"]
}
</script>

<style scoped>
div {
  border: solid 1px darkcyan;
}
</style>