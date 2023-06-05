<script>
import Stud from './components/Employee.vue'

export default {
  data() {
    return {
      
    }
  },
  components: {
    Stud
  },
  methods: {
    StudName(name) {
      console.log(name);
    },
    StudSalary(name, salary){
console.log(name, salary);
    }
  }
}

</script>

<template>
<Stud @show="StudName" @show1="StudSalary"/>
</template>

