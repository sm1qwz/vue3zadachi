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
  },
  removeProduct: function(index){
    this.products.splice(index,1);
  }
}
}
</script>

<template>
<ul>
  <li v-for="(product,index) in products" :key="index">
  {{ product }}
  <button class="greenstyle" @click="removeProduct(index)">Удалить</button>
  </li>
</ul>
</template>