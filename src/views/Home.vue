<template>
  <div class="hello">
    <h1>Home Page demon</h1>
    <home-component>
        <template v-slot:header>
            <p>This is the header slot.</p>
        </template>

        <template v-slot:footer>
            <h2>Footer slot is here.</h2>
        </template>
    </home-component>
  </div>
</template>

<script>
import HomeComponent from '../components/test/HomeComponent.vue'
export default {
  components: { HomeComponent },
  name: 'Homepage',
  props: {
    msg: String
  },
  data() {
      return {
          person: {
              title: 'Random title',
              text: 'Random text'
          }
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
