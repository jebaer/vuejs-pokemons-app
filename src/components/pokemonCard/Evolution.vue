<template>
    <p class="no-margin">
        <span class="is-bold">lvl {{ evolution.level }}: </span>{{ evolution["evolve-to"] }}
        <span class=""><img :src="evolution.image" width="25px" height="25px"/></span>
    </p>
</template>

<script>
    export default {
        name: "Evolution",
        props: {
            evolution: {
                type: Object,
                required: true
            }
        }
    }
</script>
