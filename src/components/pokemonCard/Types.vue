<template>
    <p class="no-margin is-flex-row">
        <span  v-for="type in types" v-bind:key="type" class="pokemon-type" :class="[type]">{{ type }}</span>
    </p>
</template>

<script>

    export default {
        name: "Types.vue",
        props: {
            types:{
                type: Array,
                required: true
            }
        },
    }
</script>

<style scoped>

</style>