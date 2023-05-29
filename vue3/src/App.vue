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
<p v-if="visible">Привет</p>
<button @click="toggle2">toggle</button>
<p v-if="visible2">Пока</p>
<button @click="toggle3">toggle</button>
<p v-if="visible3">Здравствуй</p>
</template>