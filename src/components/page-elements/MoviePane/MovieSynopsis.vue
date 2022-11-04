<template>
<div :style="{borderBottom: 'solid 1px ' + lineColor, color: textColor}">{{ synopsis }}</div>
</template>

<script>
export default {
  name: "MovieSynopsis",
  props: ["synopsis", "lineColor", "textColor"]
}
</script>

<style scoped>
div {
  display: grid;
  align-items: start;
  text-align: left;
  margin: 1vh;
  padding: 1vh;
  width: 90%;
  min-height: 20vh;
  height: fit-content;
}
</style>