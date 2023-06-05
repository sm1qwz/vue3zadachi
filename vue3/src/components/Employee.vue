<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {

        }
    },
    methods: {
        handleName() {
            this.$emit('show', 'Nikita Kirkitskiy');
        },
        handleSalary(){
            this.$emit('show1', 'Klim Sorokin', '10');
        }
    }
}
</script>

<template>
<button class="greenstyle" @click="handleName">Name</button>
<button class="greenstyle" @click="handleSalary">Salary</button>
</template>