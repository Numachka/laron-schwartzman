<template>
  <div class="video-container">
    <iframe
        class="video"
        src="https://www.youtube.com/embed/902Zltouttc"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
    </iframe>
  </div>
</template>

<script>
export default {
  name: "MovieVideo"
}
</script>

<style scoped>
div {
  border: solid 1px darkcyan;
}

.video-container {
  width: 100%;
  display: grid;
  justify-items: center;
  align-items: center;
}

.video {
  width: 90%;
  height: 90%;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}

</style>