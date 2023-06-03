<script>
export default{
data(){
  return{
products: ['a', 'b', 'c', 'd', 'e'],
newproduct: '',
  }
},
methods: {
  addProduct:function(){
    this.products.push(this.newProduct);
  },
  addProductEnd:function(){
    this.products.unshift(this.newProduct);
  }
}
}
</script>

<template>
<ul>
  <li v-for="(product,index) in products" :key="index">
  {{ product }}
  </li>
</ul>
<input class="inputstyle" v-model="newProduct">
<button class="greenstyle"  @click="addProduct">В конец</button>
<br>
<input class="inputstyle" v-model="newProduct">
<button class="greenstyle" @click="addProductEnd">В начало</button>
</template>