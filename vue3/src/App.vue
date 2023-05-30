<script>
export default{
  data(){
  return{
    age: 25,
  }
},
}
</script>

<template>
<p v-if ="age < 18">Подросток</p>
<p v-else-if ="19 < age && age < 25">Молодой человек</p>
<p v-else ="age > 26">Мужчина</p>
</template>