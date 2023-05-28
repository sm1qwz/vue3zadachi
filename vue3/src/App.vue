<script>
export default{
data(){
  return{
    text: "Привет",
  }
},
methods: {
	change: function() {
		this.text = "Пока";
   },
   change1: function() {
		this.text = "Опять привет";
   }
}
}

</script>

<template>
{{ text }}
<button @click="change">Меняем 1</button>
<button @click="change1">Меняем 2</button>
</template>

