<script>
export default{
data(){
  return{
    num1: 1,
    num2: 2,
    text: 'Summa'
  }
},
methods: {
  show: function(){
    let text = this.cape(this.text)
    alert(text);
  },
  cape: function(str){
    return str[0].toUpperCase() + str.slice(1);
  }
}
}
</script>

<template>
<div>{{ cape }}</div>
<div>{{ num1 + num2 }}</div>
</template>