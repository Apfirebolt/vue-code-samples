<template>
  <div class="hello">
    <slot name="header"></slot>
    <p>Content after the header named slot.</p>
    <slot name="footer"></slot>
  </div>
</template>

<script>
export default {
  name: 'HomeComponent',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
