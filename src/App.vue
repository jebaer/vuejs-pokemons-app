<template>
  <div class="grey-background" id="app">
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
    font-size: 0.9rem
    font-family: "Josefin Sans"
    color: #000
  #app
    min-height: 100vh
</style>
