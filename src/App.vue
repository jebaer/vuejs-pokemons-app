<template>
  <div class="" id="app">
    <myHeader></myHeader>
    <PokemonCard></PokemonCard>
  </div>
</template>

<script>
import myHeader from './components/Header.vue';
import PokemonCard from './components/PokemonCard.vue';

export default {
  name: 'app',
  components: {
    myHeader,
    PokemonCard
  }
}
</script>

<style lang="sass">
body
  font-size: 12px
  font-family: sans-serif
  color: #000
</style>
