<script>
import Student from './components/Employee.vue'

export default {
  data() {
    return {
      
    }
  },
  components: {
    Stud
  },
  methods: {
    Burgers() {
      alert('Hamburger, Cheeseburger, DoubleCheese');
    },
    Sandwiches(){
      alert('Roastbeef, Texas, Denmark')
    }
  }
}
</script>

<template>
<Stud @show="Burgers" @show1="Sandwiches" />
</template>
