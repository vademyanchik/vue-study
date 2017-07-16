<template>
  <footer>
    <p>{{ copyrigth }}</p>
  </footer>
</template>

<script>
export default {
  data () {
    return {
      copyrigth: '2017 '
    }
  },
}
</script>

<style scoped>
 footer {
  background: #222;
  padding: 6px;
 }

 p {
  color: lightgreen;
  text-align: center;
 }
</style>
