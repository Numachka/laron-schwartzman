<template>
  <div class="title" :style=" {borderBottom: 'solid 1px ' + lineColor}">
    <p :style="{color: titleColor}">{{ title }}</p>
  </div>
</template>

<script>
export default {
  name: "MovieTitle",
  props: ["title", "lineColor", "titleColor"]
}
</script>

<style scoped>
@font-face {
  font-family: lemon-milk;
  src: url("@/assets/fonts/LemonMilk.otf") format("opentype");
}

.title {
  display: grid;
  align-items: center;
  font-family: lemon-milk,sans-serif;
  font-size: 2rem;
  font-weight: bold;
  width: 90%;
}

</style>