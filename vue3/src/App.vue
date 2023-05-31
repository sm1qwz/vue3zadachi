<script>
export default{
data(){
  return{
    num: 0,
    res: 0,
    sum: 0,
    num1: 0,
    num2: 0,
  }
},
methods: {
  calc:function() {
    this.res = Math.sqrt(this.num);
  },
  summ:function() {
    this.sum = this.num1 + this.num2;
  }
  
}
}
</script>

<template>
<p class="pstyle">{{ res }}</p>
<input class="inputstyle" v-model="num">
<button class="greenstyle" @click="calc">work</button>
<br>
<p class="pstyle">{{ sum }}</p>
<input class="inputstyle" v-model="num1">
<input class="inputstyle" v-model="num2">
<button class="greenstyle" @click="summ">work</button>
<br>
</template>