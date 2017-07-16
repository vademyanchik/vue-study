<template>
  <div>
    <app-header></app-header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer></app-footer>
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
     ]
    }
  },
  methods: {
  },
}
</script>

<style scoped>
#app {
  background: green;
}

</style>
