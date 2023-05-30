<script>
export default{
data(){
  return{
    products: ['PC', 'Monitor', 'Keyboard'],
  }
},
methods: {
add: function(){
  this.products.push('Mouse');
},
del: function(){
  this.products.shift();
},
del1: function () {
  this.products.pop();
},
splice: function(){
  this.products.splice(2, 1);
},
sort: function(){
  this.products.sort();
},
  reverse: function () {
    this.products.reverse();
  },
}
}
</script>

<template>
<ul>
  <li v-for="elem in products">{{ elem }}</li>
</ul>
<button @click="add">Добавить продукт</button>
<br>
<button @click="del">Удалить продукт</button>
<br>
<button @click="del1">Удалить продукт в конце</button>
<br>
<button @click="splice">Удалить предпоследний продукт</button>
<br>
<button @click="sort">Отсортировать продукты</button>
<br>
<button @click="reverse">Реверс</button>
</template>
