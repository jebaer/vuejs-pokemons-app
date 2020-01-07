<template>
    <div>
        <p class="no-margin">
            <span class="is-bold">Taille: </span>{{ height }}
        </p>
        <p class="no-margin">
            <span class="is-bold">Poids: </span>{{ weight }}
        </p>
    </div>
</template>

<script>
    export default {
        name: "Measures",
        props:{
            height: {
                type: Number,
                required: true
            },
            weight: {
                type: Number,
                required: true
            }
        }
    }
</script>
