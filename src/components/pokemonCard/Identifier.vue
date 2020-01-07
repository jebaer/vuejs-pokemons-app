<template>
    <p class="is-bold no-margin">#{{ id }}
        <span class="is-text-special"> {{ name }} </span>
    </p>
</template>

<script>
    export default {
        name: "Identifier",
        props: {
            id: {
                type: Number,
                required: true
            },
            name: {
                type: String,
                required: true
            }
        }
    }
</script>
