<script>
export default{
  data(){
  return{
    isAdmin: true,
  }
},
}
</script>

<template>
<p v-if="isAdmin">Успешно</p>
<p v-else>Отказано в доступе</p>
</template>