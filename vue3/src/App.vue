<script>
import Student from './components/Employee.vue'

export default {
  data() {
    return {
      name: 'Niktia Kirkitskiy',
      salary: '1',
      age: '19',
    }
  },
  components: {
    Stud
  }
}
</script>

<template>
<Stud :name="name" :salary="salary" :age="age"/>
</template>
