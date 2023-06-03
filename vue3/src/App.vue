<script>
export default{
data(){
  return{
    text1: '',
    text2: ''
  }
},
methods: {
}
}
</script>

<template>
<input class="inputstyle" v-model="text1" v-on:keyup.enter="submit">
<button class="greenstyle" @click="toggle">toggle</button>
<p class="pstyle">{{ text1 }}</p>
<br>
<a href="#" class="inline-link1" v-on:keyup.ctlr="sub">push</a>
<p class="pstyle"></p>
</template>