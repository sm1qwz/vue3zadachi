<script>
export default {
    data() {
        return {
            newName: ' ',
            newSurn: ' ',
        }
    },
    methods: {
        save(){
            this.$emit('add', this.newName, this.newSurn)
        }
    }
}
</script>

<template>
    <input class="inputstyle" v-model="newName">
    <br>
    <br>
    <input class="inputstyle" v-model="newSurn">
    <br>
    <button class="greenstyle" @click="save">save</button>
</template>