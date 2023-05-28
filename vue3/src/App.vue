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
<div>{{ show() }}</div>
</template>