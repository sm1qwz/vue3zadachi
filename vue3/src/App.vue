<script>
import Employee from './components/Employee.vue'
import EmployeeForm from './components/EmployeeForm.vue'


export default {
  data() {
    return {
      hunters: [
        {
          id: 1,
          name: 'Alec',
          surn: 'Lightwood'
        },
        {
          id: 2,
          name: 'Jace',
          surn: 'Herondale'
        },
        {
          id: 3,
          name: 'Isabel',
          surn: 'Lightwood'
        },
      ],

    }
  },
  components: {
    Employee, EmployeeForm
  },
  methods: {
    add(name, surn){
      let id = this.hunters.length + 1;
      this.hunters.push({
        id, name, surn
      });
    }
  }
}

</script>

<template>
<EmployeeForm @add="add"/>
</template>
