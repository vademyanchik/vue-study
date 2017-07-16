<template>
  <div>
    <app-header v-bind:title="title" v-on:changeTitle="updateTitle($event)"></app-header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer v-bind:title="title"></app-footer>
  </div>  
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Ninjas from './components/Ninjas.vue';

export default {
  components: { 
    'app-header': Header,
    'app-footer': Footer,
    'app-ninjas': Ninjas,
  },
  data () {
    return {
      ninjas: [
        { name: 'Ruy', speciality: 'Vue component', show: false },
        { name: 'Ruys', speciality: 'Vue component', show: false },
        { name: 'Ruyv', speciality: 'Vue component', show: false },
        { name: 'Ruye', speciality: 'Vue component', show: false },
        { name: 'Ruyr', speciality: 'Vue component', show: false },
        { name: 'Ruyh', speciality: 'Vue component', show: false },
      ],
      title: 'Ninja',
    }
  },
  methods: {
    updateTitle: function(event) {
      this.title = event;
    },
  },
}
</script>

<style scoped>
#app {
  background: green;
}

</style>
