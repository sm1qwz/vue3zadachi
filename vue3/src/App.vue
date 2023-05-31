<script>
export default{
data(){
  return{
    selected: 'Среда',
    selectday: '31',
    selectmonth: 'Май',
    selectyear: '2023',
    options: ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье'],
    days: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30',' 31'],
    months: ['Январь', 'Февраль',
      'Март', 'Апрель', 'Май',
      'Июнь', 'Июль', 'Август', 'Сентябрь',
      'Октябрь', 'Ноябрь', 'Декабрь'],
      years: ['2023', '2022',
      '2021', '2020', '2019',
      '2018']
  }
},
methods: {
}
}
</script>

<template>
  <p class="pstyle">Какой сегодня день недели?</p>
  <select v-model="selected">
    <option v-for="option in options">{{ option }}</option>
  </select>
<br>
<br>
<p class="pstyle">Какой сегодня день месяца?</p>
<select v-model="selectday">
<option v-for="option1 in days">{{ option1 }}</option>
</select>
<br>
<br>
<p class="pstyle">Какой сегодня месяц?</p>
<select class="hunter" v-model="selectmonth">
<option v-for="option2 in months">{{ option2 }}</option>
</select>
<br>
<br>
<p class="pstyle">Какой сегодня год?</p>
<select class="hunter" v-model="selectyear">
<option v-for="option3 in years">{{ option3 }}</option>
</select>
<br>
<br>
<br>
<p class="pstyle">{{ selected }}</p>
<p class="pstyle">{{ selectday }}</p>
<p class="pstyle">{{ selectmonth }}</p>
<p class="pstyle">{{ selectyear }}</p>
</template>