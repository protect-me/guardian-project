<template>
  <div class="deck-wrapper">
    <div
      class="deck-card-wrapper"
      v-for="(character, index) in characters"
      :key="index"
    >
      <!-- class="deck-card-inner-wrapper" -->
      <deck-card :data="character"></deck-card>
    </div>
  </div>
</template>

<script>
import DeckCard from "@/components/DeckCard";

export default {
  components: {
    DeckCard,
  },
  data() {
    return {
      characters: [
        { name: "갈더", url: require("../assets/images/character/갈더.png") },
        {
          name: "나무정령",
          url: require("../assets/images/character/나무정령.png"),
        },
        {
          name: "네드웨인",
          url: require("../assets/images/character/네드웨인.png"),
        },
        {
          name: "데뉴아",
          url: require("../assets/images/character/데뉴아.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.deck-wrapper {
  border: 2px solid red;
  display: flex;
  .deck-card-wrapper {
    border: 2px solid green;
    /* .deck-card-inner-wrapper {
      border: 2px solid blue;
    } */
  }
}
</style>
