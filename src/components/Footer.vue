<template>
  <footer>
    <p>{{ title }}</p>
  </footer>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      requred: true,
    }
  },
  data () {
    return {
      copyrigth: this.title,
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
