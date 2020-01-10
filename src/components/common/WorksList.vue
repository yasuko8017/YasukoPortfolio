<script>
import WorksItem from "./WorksItem";
import axios from "axios";

export default {
  props: ['works'],
  components: {
    WorksItem,
  }
};
</script>

<template>
  <div class="worksContent">
    <WorksItem v-for="work in works" :workdata="work" />
    <div style="clear:both"></div>
  </div>
</template>

<style lang="scss" scoped>
.worksContent {
  width: 100%;
}
// PC
@media screen and (min-width: 1024px) {
}
// Pad
@media screen and (min-width: 768px) and (max-width: 1023px) {
}
// Mobile
@media screen and (max-width: 767px) {
  .worksContent {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
}
</style>
