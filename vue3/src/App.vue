<script>
export default{
data(){
  return{
    isAuth: true,
  }
},
methods: {
toggle: function(){
  this.isAuth = false;
}
}
}
</script>

<template>
  <button @click="toggle">toggle</button>
  <p v-show="isAuth">Никита Киркицкий</p>
</template>