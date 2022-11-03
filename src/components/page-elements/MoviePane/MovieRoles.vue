<template>
  <div class="role-container">
    <span v-if="direct === 'true'" class="role"><img src="@/assets/direct.svg" alt="directed"> Directed</span>
    <span v-if="produce === 'true'" class="role"><img src="@/assets/produce.svg" alt="produced"> Produced</span>
    <span v-if="edit === 'true'" class="role"><img src="@/assets/edit.svg" alt="edited"> Edited</span>
  </div>
</template>

<script>
export default {
  name: "MovieRoles",
  props: ["direct", "produce", "edit"]
}
</script>

<style scoped>
div {
  border: solid 1px darkcyan;
}

.role-container {
  display: flex;
  flex-flow: row;
}
.role {
  margin: 2vh;
  width: fit-content;
  display: flex;
  flex-flow: row;
  align-items: center;
}
</style>