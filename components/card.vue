<template>
  <div class="card">
    <span class="name">{{name}}</span>
    <img :src="image" alt="name" />
    <span class="description">{{description}}</span>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true
    },
    image: {
      type: String,
      default: "http://placehold.it/300x200"
    },
    description: {
      type: String,
      default: null
    }
  }
};
</script>

<style scoped>
.card {
  @apply rounded bg-white;

  & + .card {
    @apply ml-2;
  }
}
</style>
