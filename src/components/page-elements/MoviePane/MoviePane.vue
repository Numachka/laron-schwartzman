<template>
<div class="movie-pane">
  <movie-title title="Movie Title!"/>
  <movie-video source=""/>
  <movie-roles direct="true" produce="false" edit="true"/>
  <movie-synopsis synopsis="Curabitur venenatis sem sit amet vestibulum eleifend. Vestibulum at tellus elementum, dictum lectus nec, dignissim tellus. Aenean fermentum eleifend sollicitudin. In nec nunc et lorem auctor lacinia aliquet ut mi. Nulla tellus mi, laoreet vel neque eu, viverra finibus augue. Phasellus mollis lobortis nisi nec blandit. Aliquam lobortis blandit mi, at finibus mi luctus quis. In accumsan malesuada ipsum et mollis. Ut in justo in lectus ultrices tincidunt."/>
</div>
</template>

<script>
import MovieTitle from "@/components/page-elements/MoviePane/MovieTitle";
import MovieVideo from "@/components/page-elements/MoviePane/MovieVideo";
import MovieRoles from "@/components/page-elements/MoviePane/MovieRoles";
import MovieSynopsis from "@/components/page-elements/MoviePane/MovieSynopsis";
export default {
name: "MoviePane",
  components: {MovieSynopsis, MovieRoles, MovieVideo, MovieTitle}
}
</script>

<style scoped>
.movie-pane {
  min-height: 100vh;
  width: 100vw;
  display: grid;
  grid-template-rows: 1fr 3fr 1fr 4fr;
}
</style>