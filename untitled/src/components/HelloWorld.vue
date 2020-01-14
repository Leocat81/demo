<template>
  <div class="hello">
         {{msg}}
         <button @click.once="test">点击我</button>
 </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'sdsds'
    }
  },
  methods: {
    test () {
      console.log(typeof this.msg)
      this.msg = '里面的'
    },
    test1 () {
      this.msg = '外面的'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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
