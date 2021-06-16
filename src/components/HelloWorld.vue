<template>
  <div class="hello">
    <span id="nombre">{{ msg }}</span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
span {
  font-size: 3rem;
  color: rgb(224, 224, 224);
  padding-right: 10px;
}
h3 {
  margin: 40px 0 0;
}
</style>
