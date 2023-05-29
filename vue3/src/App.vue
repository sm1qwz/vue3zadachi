<script>
export default{
data(){
  return {
    visible: true,
    visible1: false,
  }
}
}
</script>

<template>
	<p v-if="visible">Привет</p>
  <p v-if="!visible1">Пока</p>
</template>