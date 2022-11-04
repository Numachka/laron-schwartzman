<template>
  <div class="movie-pane" :style="{background: backgroundColor}">
    <movie-title :title="title" :lineColor="lineColor" :titleColor="titleColor"/>
    <movie-video :source="source" :lineColor="lineColor"/>
    <movie-roles :direct="direct" :produce="produce" :edit="edit" :lineColor="lineColor" :titleColor="titleColor" :textColor="textColor"/>
    <movie-synopsis :synopsis="synopsis" :lineColor="lineColor" :textColor="textColor"/>
    <movie-credits :credits="credits" :lineColor="lineColor" :textColor="textColor"/>
  </div>
</template>

<script>
import MovieTitle from "@/components/page-elements/MoviePane/MovieTitle";
import MovieVideo from "@/components/page-elements/MoviePane/MovieVideo";
import MovieRoles from "@/components/page-elements/MoviePane/MovieRoles";
import MovieSynopsis from "@/components/page-elements/MoviePane/MovieSynopsis";
import MovieCredits from "@/components/page-elements/MoviePane/MovieCredits";

export default {
  name: "MoviePane",
  props: ["backgroundColor", "textColor", "title", "titleColor", "lineColor", "source", "direct", "produce", "edit", "synopsis", "credits"],
  components: {MovieSynopsis, MovieRoles, MovieVideo, MovieTitle, MovieCredits}
}
</script>

<style scoped>
.movie-pane {
  max-height: 100vh;
  max-width: 100vw;
  display: grid;
  justify-items: center;
  grid-template-rows: 1fr 3fr 1fr 3fr 1fr;
}
</style>