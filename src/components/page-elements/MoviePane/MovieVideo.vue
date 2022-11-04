<template>
  <div class="video-container" :style="{borderBottom: 'solid 1px ' + lineColor}">
    <iframe
        class="video"
        :src="source"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
    </iframe>
  </div>
</template>

<script>
export default {
  name: "MovieVideo",
  props:["source", "lineColor"]
}
</script>

<style scoped>

.video-container {
  display: grid;
  justify-items: center;
  align-items: center;
  width: 90%;
}

.video {
  width: 100%;
  height: 90%;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}

</style>