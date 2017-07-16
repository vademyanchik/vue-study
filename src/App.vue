<template>
  <div>
    <h1> {{ msg2 }} </h1>
    <p> {{ helloVueWorld() }} </p>
    <ninjas> </ninjas>
  </div> 
</template>

<script>
import Ninjas from './Ninjas.vue'

export default {
  components: { 
    'ninjas': Ninjas,
  },
  data () {
    return {
      msg: 'maxim',
      msg2: 'vadim',
    }
  },
  methods: {
    helloVueWorld: function() {
      return this.msg + this.msg2;
    },
  },
}
</script>

<style scoped>
#app {
  background: green;
}

</style>
