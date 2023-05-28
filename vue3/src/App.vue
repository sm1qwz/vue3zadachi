<script>
export default{
data(){
  return{
    cost: '100',
	amount: '10',
  }
},
computed: {
	price: function() {
		return this.cost * this.amount;
	},
	change: function() {
		this.cost = 150;
	}
}
}

</script>

<template>
<p>{{ price }}</p>
<button @click="change">Меняем цену</button>
</template>

