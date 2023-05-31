<script>
export default{
data(){
  return{
    selected: ' ',
  }
},
methods: {
vis(){
      this.visible = true;
},
  vis1() {
    this.visible1 = true;
  },
  vis2() {
    this.visible2 = true;
  }
}
}
</script>

<template>
    <p class ='pstyle'>В каком городе вы живете?</p>
    <select v-model="selected">
		<option>Симферополь</option>
		<option>Севастополь</option>
		<option>Евпатория</option>
	</select>
	
	<p class ='pstyle'>{{ selected }}</p>
</template>