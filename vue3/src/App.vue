<script>
export default{
  data(){
  return{
    visible: true,
    visible2: true,
    visible3: true,
  }
},
methods: {
  toggle: function(){
    this.visible = !this.visible;
  },
  toggle2: function () {
    this.visible2 = !this.visible2;
  },
  toggle3: function () {
    this.visible3 = !this.visible3;
  }
}
}
</script>

<template>
<button @click="toggle">toggle</button>
<p>{{visible ? 'Никита' : 'Киркицкий'}}</p>
<button @click="toggle1">toggle</button>
<p>{{visible1 ? 'Клим' : 'Сорокин'}}</p>
<button @click="toggle2">toggle</button>
<p>{{visible2 ? 'Мавиле' : 'Бекирова'}}</p>
</template>