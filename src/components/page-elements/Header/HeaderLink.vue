<template>
  <span>
    <a :href="action">
      <img alt="header link" :src="require(`@/assets/${imageSource}`)">
    </a>
  </span>
</template>

<script>
export default {
  name: "HeaderLink",
  props: ["type", "action", "imageSource"]
}
</script>

<style scoped>
span {
  margin: 1vh;
}
</style>