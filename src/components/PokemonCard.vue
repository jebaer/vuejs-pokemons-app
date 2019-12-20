<template>
  <section class="container">

    <div class="is-mobile columns pokemon-card is-vcentered">

      <div class="column">
        <img :src="pokemon[0].image"/>
      </div>

      <div class="column">
        <div class="is-flex">
          <p id="pokemon-id">#{{ pokemon[0].id }}</p>
          <p class="has-text-link is-uppercase is-bold">{{ pokemon[0].name }}</p>
        </div>
        <p>Poids: {{ pokemon[0].height}}</p>
        <p>Taille: {{ pokemon[0].weight }}</p>
        <p>Type: {{ pokemon[0].types }}</p>
        <p>lvl {{ pokemon[0].evolve.level }}: {{ pokemon[0].evolve["evolve-to"] }}
          <span class="evol-pokemon"><img :src="pokemon[0].evolve.image" width="25px" height="25px"/></span>
        </p>
      </div>

    </div>

  </section>
</template>

<script>
import Pokemons from "../assets/mock_pokemons.json"

export default {
  name: "pokemonCard",
  data() {
    return {
      pokemon: Pokemons
    }
  }
}
</script>

<style lang="sass">
  .pokemon-card
    margin: 25px
    background-color: lighten(#E6EBE0, 5%)

  #pokemon-id
    margin-right: 15px
</style>
