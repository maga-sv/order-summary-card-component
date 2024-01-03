<script setup>
import BgPatternDesc from './assets/images/BgPatternDesc.vue';
import Card from './components/card/Card.vue';

</script>

<template>

<main>

  <BgPatternDesc class="bg" />

  <section class="order">

    <div class="container">

      <Card />

    </div>

  </section>

</main>

</template>

<style lang="scss" scoped>

main {
  height: 100vh;
  position: relative;
  display: grid;
  place-items: center;

  .bg {
    top: 0;
    left: 0;
    position: absolute;
    width: 100%;
    z-index: -1;
  }
}

</style>
