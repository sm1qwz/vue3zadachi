<script>
import Stud from './components/Employee.vue'

export default {
  data() {
    return {
      hunters: [
        {
          id: 1,
          name: 'Nikita',
          surn: 'Kirkitskiy'
        },
        {
          id: 2,
          name: 'Klim',
          surn: 'Sorokin'
        },
        {
          id: 3,
          name: 'Mavile',
          surn: 'Bekirova'
        },
      ],

    }
  },
  components: {
    Stud
  },
  methods: {
    change(id, name, surn){
      this.hunters = this.hunters.map((hunter) => {
        if(hunter.id === id){
          hunter.name = name;
          hunter.surn = surn;
        }
        return hunter;
      });
    }
  }
}

</script>

<template>
<Stud v-for   ="hunter in hunters"
		:id     ="hunter.id"
		:name   ="hunter.name"
		:surn   ="hunter.surn"
		:key    ="hunter.id"
    @change="change"/>
</template>
