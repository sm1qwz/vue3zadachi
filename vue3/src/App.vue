<script>
import Student from './components/Employee.vue'

export default {
  data() {
    return {
      students: [
        {
          id: 1,
          name: 'Nikita',
          salary: 10,
          age: 19
        },
        {
          id: 2,
          name: 'Klim',
          salary: 11,
          age: 18
        },
        {
          id: 3,
          name: 'Emran',
          salary: 500000,
          age: 19
        },
      ],
    }
  },
  components: {
    Stud
  }
}
</script>

<template>
<Stud v-for="student in students" :name="student.name" :salary="student.salary" :age="student.age" :key="student.id" />
</template>
