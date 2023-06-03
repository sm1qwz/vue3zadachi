<script>
export default{
data(){
  return{
    students: [
      {
        id: 1,
        name: 'Nikita Kirkistkiy',
        mark: 4,
        age: 19,
      },
      {
        id: 2,
        name: 'Mavile Bekirova',
        mark: 5,
        age: 19,
      },
      {
        id: 3,
        name: 'Klim Sorokin',
        mark: 3,
        age: 18,
      },
    ]
  }
},
methods: {
  edit(student){
    student.isEdit = true;
  },
  save(student){
    student.isEdit = false;
  },
}
}
</script>

<template>
<table>
<tr v-for="student in student" :key="student.id"> 
<template v-if="!student.isEdit">
  {{ student.name }} {{ student.mark }} {{ student.age }}<button class="greenstyle" @click="edit(student)">edit</button>
</template>
<template v-else>
  <input v-model="student.name">
  <input v-model="student.mark">
  <input v-model="student.age">
  <button class="greenstyle" @click="save(student)">
      save
  </button>
</template>
</tr>
</table>
</template>