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
    ],
  }
},
methods: {
  removeStudent: function (id) {
    this.students = this.students.filter((student) => {
      return student.id !== id;
    })
  }
}
}
</script>

<template>
<table>
  <tr v-for="student in students" :key="student.id"> {{ student.name }} {{ student.mark }} {{ student.age }}<button class="greenstyle" @click="removeStudent(students.id)">Убрать</button>
</tr>
</table>
</template>