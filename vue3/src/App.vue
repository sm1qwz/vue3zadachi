<script>
export default{
data(){
  return{
    arr: ['x', 'y', 'z'],
  }
},
methods: {
}
}
</script>

<template>
   <ul v-for="(elem,key) in arr">{{ key }}</ul>
</template>