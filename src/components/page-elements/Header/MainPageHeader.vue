<template>
  <header>
    <header-link type="phone" action="tel:0524330984" image-source="call.svg"/>
    <header-link type="email" action="mailto:numachka@gmail.com" image-source="directbox.svg"/>
    <header-link type="whatsapp" action="" image-source="whatsapp.svg"/>
    <header-link type="youtube" action="https://youtube.com" image-source="youtube.svg"/>
  </header>
</template>

<script>
import HeaderLink from "@/components/page-elements/Header/HeaderLink";
export default {
  name: "MainPageHeader",
  components: {HeaderLink}
}
</script>

<style scoped>
header {
  display: flex;
  flex-flow: column;
  width: fit-content;
  position: absolute;
  margin: 1vh;
  padding: 0.5vh;
  background: rgba(0, 0, 0, 0.12);
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  z-index: 1;
}
</style>