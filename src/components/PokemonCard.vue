<template>
  <section class="container is-center">

    <div class="card is-quarter is-flex-row" v-for="pokemon in pokemons" :key="pokemon.id">

      <div class="is-flex-column is-justify-center is-align-centered is-flex-grow is-margin-right-20">
        <img :src="pokemon.image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center details">
        <Identifier :id="pokemon.id" :name="pokemon.name"></Identifier>
        <Measures :height="pokemon.height" :weight="pokemon.weight"></Measures>
        <Types :types="pokemon.types"></Types>
        <Evolution :evolution="pokemon.evolve"></Evolution>
      </div>

    </div>

  </section>
</template>

<script>
import Pokemons from "../assets/mock_pokemons.json"
import Evolution from "./pokemonCard/Evolution";
import Identifier from "./pokemonCard/Identifier";
import Types from "./pokemonCard/Types";
import Measures from "./pokemonCard/Measures";

export default {
  name: "pokemonCard",
  components: {
    Evolution,
    Identifier,
    Measures,
    Types
  },
  data() {
    return {
      pokemons: Pokemons
    }
  }
}
</script>

