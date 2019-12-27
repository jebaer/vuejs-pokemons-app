<template>
  <section class="container is-center">

    <div class="card is-quarter is-flex-row" v-for="pokemon in pokemons" :key="pokemon.id">

      <div class="is-flex-column is-justify-center is-align-centered is-flex-grow">
        <img :src="pokemon.image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center details">
        <p class="is-bold no-margin">#{{ pokemon.id }}
          <span class="is-text-special"> {{ pokemon.name }} </span>
        </p>
        <p class="no-margin">
          <span class="is-bold">Poids: </span>{{ pokemon.height}}
        </p>
        <p class="no-margin">
          <span class="is-bold">Taille: </span>{{ pokemon.weight }}
        </p>
        <p class="no-margin">
          <span class="is-bold">Type: </span>{{ pokemon.types }}
        </p>
        <p class="no-margin">
          <span class="is-bold">lvl {{ pokemon.evolve.level }}: </span>{{ pokemon.evolve["evolve-to"] }}
          <span class=""><img :src="pokemon.evolve.image" width="25px" height="25px"/></span>
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
      pokemons: Pokemons
    }
  }
}
</script>

