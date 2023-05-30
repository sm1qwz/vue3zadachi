<script>
export default{
  data(){
  return{
    visible: true,
btnHide: true,
btnVis: false,
  }
},
methods: {
  hide: function(){
    this.visible = false;
    this.btnHide = false;
    this.btnVis = true;
  },
  vis: function(){
    this.visible = true;
    this.btnHide = true;
    this.btnVis = false;
  }
}
}
</script>

<template>
<button class="greenstyle" @click="hide" v-if="btnHide">Скрыть</button>
<button class="greenstyle" @click="vis" v-if="btnVis">Показать</button>
<p v-if="visible">Привет</p>
</template>