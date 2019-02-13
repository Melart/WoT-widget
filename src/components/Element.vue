<template>
  <button>{{msg}}</button>
</template>

<script>
export default {
  name: 'Element',
  props: {
    msg: String
  }
}

</script>

<style scoped>
    button {
        background: black;
        color: #fff;
        width: 137px;
        height: 40px;
        margin-right: 12px;
    }
</style>
