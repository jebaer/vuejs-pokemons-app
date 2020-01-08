<template>
    <div>
        <p class="no-margin">
            <span class="is-bold">Taille: </span>{{ convertHeight }} m
        </p>
        <p class="no-margin">
            <span class="is-bold">Poids: </span>{{ convertWeight }} kg
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
        },
        computed:{
            convertHeight() {
                return Math.floor(this.height * 10 )  / 100 ;
            },
            convertWeight() {
                return Math.floor( this.weight * 10 )  / 100  ;
            }
        }
    }
</script>
