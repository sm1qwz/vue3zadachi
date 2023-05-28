<script>
export default{
data(){
  return{
    date: '1'
  }
},
methods: {
  show: function(){
    let date = this.dayOfWeek(this.date);
    alert(date);
  },
  dayOfWeek: function(date){
    let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    return days[date];
  },
  main: function(){
    const dayOfWeekDigit = new Date().getDay();
    let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    return dayOfWeekDigit[days]
  },
   }
}

</script>

<template>
<button @click="show">Текущий день недели</button>
{{ dayOfWeekDigit }}
</template>

