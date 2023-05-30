<script>
export default{
data(){
  return{
    obj: {
	user1: '100$',
	user2: '200$',
	user3: '300$',
},
  }
},
methods: {
}
}
</script>

<template>
 <ul>
    <li v-for="elem in obj">{{ elem }}</li>
  </ul>
  <br>
  <br>
  <ul>
    <li v-for="(key, elem) in obj"> {{ elem }} - {{ key }}</li>
  </ul>
  <br>
  <br>
  <ul>
    <li v-for="(key, elem, index) in obj"> {{ elem }} - {{ key }} - {{ index }}</li>
  </ul>
  <br>
  <br>
  <ul>
    <li v-for="(key, elem, index) in obj"> {{ elem }} - {{ key }} - {{ index+1 }}</li>
  </ul>
</template>