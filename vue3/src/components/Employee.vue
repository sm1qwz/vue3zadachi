<script>
export default {
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['remove'],
    data() {
        return {

        }
    },
    methods: {
    }
}
</script>

<template>
    <p class="greenstyle">{{ name }} {{ surn }}</p>
    <button class="greenstyle" @click="$emit('remove', id)">
        remove
    </button>
</template>