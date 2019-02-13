<template>
  <div class="element-selection">
    <h1>{{ msg }}</h1>
    <p>
      На данный момент у вас выбрано {{0+2}} элементов
    </p>
  </div>
</template>

<script>
export default {
  name: 'Section',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
h1 {
  margin: 0;
  padding: 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
