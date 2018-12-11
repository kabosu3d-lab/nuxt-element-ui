<template>
  <div class="star">
    <el-rate v-model="value" :colors="['#2F3D4D', '#64B486', '#4B7C6E']">f</el-rate>
  </div>
</template>
<script lang="ts">
import { Component, Prop, Vue } from "nuxt-property-decorator";

@Component({})
export default class Star extends Vue {}
</script>
<style scoped>
.star {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  padding: 1rem;
  margin: 0.25rem;
  border: 0.25rem solid gainsboro;
}
</style>
