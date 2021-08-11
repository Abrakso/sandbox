<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>
    <i>
      r<sub>i</sub> = (d + (P<sub>i</sub> - P<sub>0</sub>)) / P<sub>0</sub> &times; 100
    </i>
    </h2>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
