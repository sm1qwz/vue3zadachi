<script>
export default{
  data(){
  return{
    visible: true,
    styles: {
      hidden: true,
    },
  }
},
methods: {
setDone:function(){
  this.styles.hidden = false;
},
setTwo: function(){
  this.styles.hidden = true;
},
  toggle: function () {
    this.visible = !this.visible;
  }
}
}
</script>

<template>
<button class="greenstyle" @click="toggle">toggle</button>
<p class="{active: true, valid: false}" v-if="visible">Привет</p>
<p :class="styles">Пока</p>
<button class="greenstyle" @click="setDone">visible</button>
<button class="greenstyle" @click="setTwo">hide</button>
</template>

<style>
p.hidden{
  display: none;
}
</style>