<script>
export default {
    emits: ['show'],
    data() {
        return {

        }
    },
    methods: {
    }
}
</script>

<template>
<button class="greenstyle" @click="$emit('show', 'Nikita Kirkitskiy')">Name</button>
</template>