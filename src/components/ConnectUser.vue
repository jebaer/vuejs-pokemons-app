<template>
  <div class="is-flex-column is-align-centered is-justify-center">
    <div @click="connectUser()" class="clickable">
      <span class="circle-wrapper"  v-bind:class="{connected: connected}"></span>
    </div>
    <p  class="is-text-special no-margin">
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
  div
    min-width: 70px

  span.circle-wrapper
    display: inline-flex
    margin-left: 17px
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
