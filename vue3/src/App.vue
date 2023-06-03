<script>
export default{
data(){
  return{
    isDisabled: true,
    isDisabled1: true,
    checked: false,
  }
},
methods: {
  toggle: function(){
    this.isDisabled = false;
  },
  toggle1: function(){
    this.isDisabled1 - false;
  },
}
}
</script>

<template>
<input class="inputstyle" type="text" v-bind:disabled="isDisabled">
<button class="greenstyle" @click="toggle">toggle</button>
<br>
<br>
<input class="inputstyle" type="text" v-bind:disabled="isDisabled1">
<br>
<input type="checkbox" v-model="checked" @click="toogle1">
</template>