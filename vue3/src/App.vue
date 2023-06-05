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
    remove(id) {
      this.hunters = this.hunters.filter((hunter) => {
        return hunter.id !== id;
      })
    }
  }
}

</script>

<template>
<Stud v-for   ="hunter in hunters"
		:id     ="hunter.id"
		:name   ="hunter.name"
		:surn   ="hunter.surn"
		@remove ="remove"
		:key    ="hunter.id"/>
</template>

