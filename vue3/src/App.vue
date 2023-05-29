<script>
export default{
data(){
  return {
    hidden: false,
  }
}
}
</script>

<template>
	<p v-if="!hidden">Привет</p>
</template>