<script>
export default{
data(){
  return{
    date: '1'
  }
},
methods: {
	show: function(str) {
		alert(str*str)
   }
},
}


</script>

<template>
<button @click="show(2)">Квадрат числа 2</button>
<button @click="show(3)">Квадрат числа 3</button>
</template>

