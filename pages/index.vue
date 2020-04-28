<template>
  <div class="main-container h-screen items-center justify-center flex">
    <div class="text-center">
      <h1 class="text-white font-mono mb-8">Untitled Card Game</h1>
      <br />
      <n-link to="/game" class="btn btn-blue">Start Game</n-link>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style scoped>
.main-container {
  background-image: url("https://i.pinimg.com/originals/f3/64/b7/f364b7d0a49566891789d291b8b2e53f.png");
}
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
