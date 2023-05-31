<script>
export default{
data(){
  return{
    message: 'hello',
    number: '5',
  }
},
methods: {
}
}
</script>

<template>
<input v-model="message">
<p class="pstyle" :style="{textTransform: 'uppercase'}">{{ message }}</p>
<br>
<input v-model="number">
<p class="pstyle">{{ number*number }}</p>
</template>