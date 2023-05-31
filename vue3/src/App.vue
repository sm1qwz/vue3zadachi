<script>
export default{
data(){
  return{
    language: '',
    visible: false,
    visible1: false,
    visible2: false,
  }
},
methods: {
vis(){
      this.visible = true;
},
  vis1() {
    this.visible1 = true;
  },
  vis2() {
    this.visible2 = true;
  }
}
}
</script>

<template>
<div>
<p>Какой язык ваш родной?</p>
<input name="radio" type="radio" v-model="language" value="Русский" @click="vis">
<label for="">Русский?</label>
<br>
<input name="radio" type="radio" v-model="language" value="Украинский" @click="vis1">
<label for="">Украинский?</label>
<br>
<input name="radio" type="radio" v-model="language" value="Беларусский" @click="vis2">
<label for="">Беларусский?</label>
</div>
<p v-if="visible">Привет</p>
<p v-else-if="visible1">Привiт</p>
<p v-else-if="visible2">Прывітанне</p>
<p v-else=''> </p>

<p>Ваш выбор: {{ language }}</p>
<br>
</template>