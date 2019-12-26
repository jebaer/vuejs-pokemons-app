<template>
<header class="is-flex-row blue-background is-justify-between">
  <Title></Title>
  <ConnectUser></ConnectUser>
</header>
</template>

<script>
  import ConnectUser from "./ConnectUser.vue"
  import Title from "./Title.vue"
  export default {
    name: "myHeader",
    components: {
      ConnectUser,
      Title
    }
  }
</script>

<style lang="sass">
  header
    padding: 15px
</style>
