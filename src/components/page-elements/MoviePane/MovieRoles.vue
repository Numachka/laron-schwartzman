<template>
  <div class="role-container" :style="{borderBottom: 'solid 1px ' + lineColor, color: textColor}">
    <span v-if="direct === 'true'" class="role"><produce-icon :color="titleColor"/>&nbsp;Produced</span>
    <span v-if="produce === 'true'" class="role"><direct-icon :color="titleColor"/>&nbsp;Directed</span>
    <span v-if="edit === 'true'" class="role"><edit-icon :color="titleColor"/>&nbsp;Edited</span>
  </div>
</template>

<script>
import ProduceIcon from "@/components/page-elements/MoviePane/CreditIcons/ProduceIcon"
import DirectIcon from "@/components/page-elements/MoviePane/CreditIcons/DirectIcon"
import EditIcon from "@/components/page-elements/MoviePane/CreditIcons/EditIcon"
export default {
  name: "MovieRoles",
  components: {ProduceIcon, DirectIcon, EditIcon},
  props: ["direct", "produce", "edit", "lineColor", "titleColor", "textColor"]
}
</script>

<style scoped>

.role-container {
  display: flex;
  flex-flow: row;
  justify-content: center;
  width: 90%;
}

.role {
  margin: 1vh;
  width: fit-content;
  display: flex;
  flex-flow: row;
  align-items: center;
}
</style>