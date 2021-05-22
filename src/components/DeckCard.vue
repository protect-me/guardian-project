<template>
  <div>
    <v-card class="deck-card-inner-wrapper">
      <v-img :src="data.url" width="100px"></v-img>
      <v-card>{{ data.name }}</v-card>
    </v-card>
  </div>
</template>

<script>
export default {
  props: ["data"],
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.deck-card-inner-wrapper {
  padding: 20px;
}
</style>
