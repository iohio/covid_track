<template>
  <div class="hello">
    <h1 v-if="Me">{{ msg }}</h1>
    <button @click="hello">Click Me</button>
    <User name="lnwmee" bio="meeza meeza meeza"/>
  </div>
</template>

<script>
import User from './User.vue'
export default {
  name: 'HelloWorld',
  data () {
    return {
      Me: true,
      msg: 'Hello Nakit'
    }
  },
  methods: {
    hello: function () {
      this.msg = 'Thank you for click on me :)'
    }
  },
  components: {
    User
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
