<template>
  <main-page-header/>
  <movie-pane/>
  <main-page-footer/>
</template>

<script>
import MoviePane from "@/components/page-elements/MoviePane/MoviePane";
import MainPageHeader from "@/components/page-elements/Header/MainPageHeader";
import MainPageFooter from "@/components/page-elements/Footer/MainPageFooter";
export default {
  name: "MainPage",
  components: {MainPageFooter, MainPageHeader, MoviePane}
}
</script>

<style scoped>

</style>