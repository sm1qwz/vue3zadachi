<script>
export default{
data(){
  
},
methods: {
  show: function(){
    alert(new Date().toLocaleDateString());
  }
}
}
</script>

<template>
<button @click="show">Текущая дата</button>
<button @mouseover="show">Текущая дата мышкой</button>
</template>