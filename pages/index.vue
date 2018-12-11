<template>
  <section>
    <Star></Star>
    <Card v-for="person in people" :key="person.id" :person="person"></Card>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";
import { State } from "vuex-class";
import Card from "~/components/Card.vue";
import Star from "~/components/Star.vue";

@Component({
  components: {
    Star,
    Card
  }
})
export default class extends Vue {
  @State people;
}
</script>
<style scoped>
.header {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

.cards {
  display: flex;
  flex-wrap: wrap;
}
</style>