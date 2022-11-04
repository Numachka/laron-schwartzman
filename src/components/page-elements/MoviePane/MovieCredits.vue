<template>
  <div :style="{borderBottom: 'solid 1px ' + lineColor, color: textColor}">{{ credits }}</div>
</template>

<script>
export default {
  name: "MovieCredits",
  props: ["credits", "lineColor", "textColor"]
}
</script>

<style scoped>
div {
  display: grid;
  align-items: start;
  margin: 1vh;
  padding: 1vh;
  width: 90%;
  min-height: 10vh;
  height: fit-content;
}
</style>