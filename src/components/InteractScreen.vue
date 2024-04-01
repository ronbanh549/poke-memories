<template>
  <div class="screen">
    <h1>Ineract Components here...</h1>
    <card-flip v-for="(card, index) in cardContext" :key="index" />
  </div>
</template>

<script>
import CardFlip from "./AppCard.vue";
export default {
  props: {
    cardsContext: {
      type: Array,
      default: function () {
        return [];
      },
    },
  },
  components: {
    CardFlip,
  },
};
</script>
