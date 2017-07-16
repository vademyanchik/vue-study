<template>
<div>
  <h1> List of NInjas </h1>
  <ul>
    <li v-for="ninja in ninjas">{{ ninja }}</li>
  </ul>
</div> 
</template>

<script>
export default {
  data () {
    return {
      ninjas: [ 'MAXIM', 'maxim', 'dima' ]
    }
  },
}
</script>

<style scoped>
 h1 { 
   color: red;  
 }

 li {
   color: green;  
 }
</style>
