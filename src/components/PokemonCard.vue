<template>
  <section class="container is-center">
      <div class="card is-quarter is-flex-row">

        <div class="is-flex-column is-justify-center is-align-centered is-flex-grow">
          <img :src="pokemon[0].image"  width="100px" height="100px"/>
        </div>

        <div class="is-flex-column is-justify-center details">
          <p class="is-bold">#{{ pokemon[0].id }}
            <span class="is-text-special"> {{ pokemon[0].name }} </span>
          </p>
          <p ><span class="is-bold">Poids: </span>{{ pokemon[0].height}}</p>
          <p><span class="is-bold">Taille: </span>{{ pokemon[0].weight }}</p>
          <p><span class="is-bold">Type: </span>{{ pokemon[0].types }}</p>
          <p><span class="is-bold">lvl {{ pokemon[0].evolve.level }}: </span>{{ pokemon[0].evolve["evolve-to"] }}
            <span class="evol-pokemon"><img :src="pokemon[0].evolve.image" width="25px" height="25px"/></span>
          </p>
        </div>

      </div>

    <div class="card is-quarter is-flex-row">

      <div class="is-flex-column is-justify-center">
        <img :src="pokemon[0].image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center">
        <p id="pokemon-id">#{{ pokemon[0].id }}
          <span class="has-text-link is-uppercase is-bold"> {{ pokemon[0].name }} </span>
        </p>
        <p>Poids: {{ pokemon[0].height}}</p>
        <p>Taille: {{ pokemon[0].weight }}</p>
        <p>Type: {{ pokemon[0].types }}</p>
        <p>lvl {{ pokemon[0].evolve.level }}: {{ pokemon[0].evolve["evolve-to"] }}
          <span class="evol-pokemon"><img :src="pokemon[0].evolve.image" width="25px" height="25px"/></span>
        </p>
      </div>

    </div>

    <div class="card is-quarter is-flex-row">

      <div class="is-flex-column is-justify-center">
        <img :src="pokemon[0].image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center">
        <p id="pokemon-id">#{{ pokemon[0].id }}
          <span class="has-text-link is-uppercase is-bold"> {{ pokemon[0].name }} </span>
        </p>
        <p>Poids: {{ pokemon[0].height}}</p>
        <p>Taille: {{ pokemon[0].weight }}</p>
        <p>Type: {{ pokemon[0].types }}</p>
        <p>lvl {{ pokemon[0].evolve.level }}: {{ pokemon[0].evolve["evolve-to"] }}
          <span class="evol-pokemon"><img :src="pokemon[0].evolve.image" width="25px" height="25px"/></span>
        </p>
      </div>

    </div>

    <div class="card is-quarter is-flex-row">

      <div class="is-flex-column is-justify-center">
        <img :src="pokemon[0].image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center">
        <p id="pokemon-id">#{{ pokemon[0].id }}
          <span class="has-text-link is-uppercase is-bold"> {{ pokemon[0].name }} </span>
        </p>
        <p>Poids: {{ pokemon[0].height}}</p>
        <p>Taille: {{ pokemon[0].weight }}</p>
        <p>Type: {{ pokemon[0].types }}</p>
        <p>lvl {{ pokemon[0].evolve.level }}: {{ pokemon[0].evolve["evolve-to"] }}
          <span class="evol-pokemon"><img :src="pokemon[0].evolve.image" width="25px" height="25px"/></span>
        </p>
      </div>

    </div>

    <div class="card is-quarter is-flex-row">

      <div class="is-flex-column is-justify-center">
        <img :src="pokemon[0].image"  width="100px" height="100px"/>
      </div>

      <div class="is-flex-column is-justify-center">
        <p id="pokemon-id">#{{ pokemon[0].id }}
          <span class="has-text-link is-uppercase is-bold"> {{ pokemon[0].name }} </span>
        </p>
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
</style>
