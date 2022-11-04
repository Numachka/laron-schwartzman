<template>
  <main-page-header/>
  <movie-pane
      backgroundColor="#050403"
      textColor="#948386"
      lineColor="#CA9655"
      titleColor="#AB382B"
      title="CROWS"
      source="https://www.youtube.com/embed/tGjGq7RDWMI"
      direct="true"
      produce="true"
      edit="true"
      synopsis="A young dude trying to understand what tht hell is going on"
      credits="With David Bar Ilan | Eldad Ben-Tora | DOP Din Barenboim | Edito Alon Duchovni | Producers Roi Kochavi & Laron Schwartzman | AD Jonathan Weitz | Original Music Yoni Shalev | Director and Writer Laron Schwartzman"
  />
  <movie-pane
      backgroundColor="#091215"
      textColor="#91A1A4"
      lineColor="#76A3B2"
      titleColor="#43C2B9"
      title="JOHN WICK"
      source="https://www.youtube.com/embed/C0BMx-qxsP4"
      direct="true"
      produce="false"
      edit="true"
      synopsis="An ex-hitman comes out of retirement to track down the gangsters that took everything from him. With New York City as his bullet-riddled playground, JOHN WICK (Keanu Reeves) is a fresh and stylized take on the assassin genre."
      credits="Keanu Reeves | and Friends"
  />
  <movie-pane
      backgroundColor="#292133"
      textColor="#82A1CA"
      lineColor="#686DA9"
      titleColor="#C181A6"
      title="OBI WAN KENOBI"
      source="https://www.youtube.com/embed/3Yh_6_zItPU"
      direct="true"
      produce="false"
      edit="true"
      synopsis="The story begins 10 years after the dramatic events of “Star Wars: Revenge of the Sith” where Obi-Wan Kenobi faced his greatest defeat—the downfall and corruption of his best friend and Jedi apprentice, Anakin Skywalker, who turned to the dark side as evil Sith Lord Darth Vader.
The series stars Ewan McGregor, reprising his role as the iconic Jedi Master, and also marks the return of Hayden Christensen in the role of Darth Vader."
      credits="Liam Nissan | and Friends"
  />
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