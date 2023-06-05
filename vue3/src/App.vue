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
StudName(name){
  console.log(name);
},
  }
}

</script>

<template>
<Stud @show="StudName"/> 
</template>

