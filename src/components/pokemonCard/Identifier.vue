<template>
    <p class="is-bold no-margin">#{{ getId() }}
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
        },
        methods: {
            getId() {
                return this.id < 10 ? `00${this.id}` : this.id < 100 ? `0${this.id}` : this.id;
            }
        }
    }
</script>
