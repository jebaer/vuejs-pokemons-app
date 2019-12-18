<template>
<header class="columns  is-mobile is-vcentered has-background-primary">

  <div class="column is-three-quarters has-text-left">
    <h1 class="has-text-link is-size-4 is-family-primary"> Pokevue!</h1>
    <h2 class="has-text-light is-size-6 is-family-primary"> Attrapez les tous. </h2>
  </div>

  <div class="column has-text-centered">
    <div @click="connectUser()" class="is-inline-flex">
      <span class="circle-wrapper"  v-bind:class="{connected: connected}"></span>
    </div>
    <p  class="has-text-link is-half">
      <span v-if="connected">{{ playerName }}</span>
      <span v-else> Inconnu </span>
    </p>
  </div>

</header>
</template>

<script>
  export default {
    name: "myHeader",
    data() {
      return {
        playerName: "Sacha",
        connected: false
      }
    },
    methods: {
      connectUser(){
        this.connected = !this.connected;
      }
    }
  }
</script>

<style lang="sass">
  header
    padding: 15px
    div
      div
        .circle-wrapper
          min-width: 30px
          max-width: 30px
          min-height: 30px
          border: solid 3px #ED6A5A
          border-radius: 50%
          background-color:  #E6EBE0
        .connected
          border: solid 3px #03CEA4
      p
        min-height: 25px
</style>
