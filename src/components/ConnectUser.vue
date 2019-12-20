<template>
  <div class="column has-text-centered">
    <div @click="connectUser()" class="is-inline-flex">
      <span class="circle-wrapper"  v-bind:class="{connected: connected}"></span>
    </div>
    <p  class="has-text-link is-half">
      <span v-if="connected">{{ playerName }}</span>
      <span v-else> Inconnu </span>
    </p>
  </div>
</template>

<script>

export default {
  name: "ConnectUser",
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
  span.circle-wrapper
    min-width: 30px
    max-width: 30px
    min-height: 30px
    border: solid 3px #ED6A5A
    border-radius: 50%
    background-color:  #E6EBE0
  span.connected
    border: solid 3px #03CEA4
  p
    min-height: 25px
</style>
