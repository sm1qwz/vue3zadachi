<script>
export default{
data(){
  
},
methods: {
  show: function(){
    alert(new Date().toLocaleDateString());
  }
}
}
</script>

<template>
<a href="https://github.com/sm1qwz/vue3zadachi" onclick="event.preventDefault()">Ссылка</a>
<br>
<br>
<button @click.once="show">Текущая дата</button>
</template>
