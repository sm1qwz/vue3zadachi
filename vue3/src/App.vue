<script>
export default{
data(){
  return{
    checked: true,
    visible: true,
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
<input class="inputstyle" type="checkbox" v-model="checked">
<button class="greenstyle" @click="ltoggle">toggle</button>
<p class="pstyle" v-if="visible">{{ checked ? 'yes' : 'no' }}</p>
</template>