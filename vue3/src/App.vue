<script>
export default{
data(){
  return{
    arr: [],
  }
},
methods: {
ltoggle: function(){
  this.checked = false;
  this.visible = !this.visible;
}
}
}
</script>

<template>
  <div>
<input class="inputstyle" type="checkbox" v-model="arr" value="Vue3">
<label>Vue3?</label>
<br>
<input class="inputstyle" type="checkbox" v-model="arr" value="Js">
<label>JavaScript?</label>
<br>
<input class="inputstyle" type="checkbox" v-model="arr" value="CSS">
<label>CSS?</label>
<ol>
  <li v-for="elem in arr">{{ elem }}</li>
</ol>
</div>
<br>
</template>