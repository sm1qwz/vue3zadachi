<script>
export default{
data(){
  return{
    items: [1, 2, 3],
  }
},
methods: {
}
}
</script>

<template>
<div v-for="elem in items">
  <p>{{ elem }}</p>
  <p class="divider"> </p>
  </div>
  <br>
  <ul v-for="elem in items">
    <li>{{ elem }}</li>
    <li class="divider"> </li>
  </ul>
</template>