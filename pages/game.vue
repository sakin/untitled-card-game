<template>
  <div class="main-container h-screen flex justify-center">
    <div class="game-cards flex self-end">
      <card v-for="card in cards" v-bind="card" v-bind:key="card.id"></card>
    </div>
  </div>
</template>

<script>
import Card from "~/components/card.vue";

const CARDS = [
  {
    id: 1,
    name: "Card 1",
    description: "I'm the very first card!"
  },
  {
    id: 2,
    name: "Card 2",
    description: "I'm the 2nd card"
  }
];

export default {
  components: {
    Card
  },
  data() {
    return {
      cards: CARDS
    };
  }
};
</script>

<style lang="postcss">
.main-container {
  background-image: url("~assets/images/y-so-serious.png");
}
</style>
