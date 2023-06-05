<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {

        }
    },
    methods: {
        handle1() {
            this.$emit('show');
        },
        handle2() {
            this.$emit('show1');
        },
    }
}
</script>

<template>
<button class="greenstyle" @click="handle1">Burgers</button>
<button class="greenstyle" @click="handle2">Sandwiches</button>
    </template>