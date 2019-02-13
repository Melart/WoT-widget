<template>
    <button>{{msg}}</button>
</template>
<script>
  export default {
    name: 'OpenPopup',
    props: {
      msg: String
    }
  }
</script>

<style scoped>
    button {
        background: #9ca85a;
        color: #000;
        width: 157px;
        height: 40px;
        margin-top: 20px;
    }
</style>