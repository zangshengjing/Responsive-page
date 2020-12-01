<template>
  <div class="container">
    <div style="background: blue">1</div>
    <div style="background: orange">2</div>
    <div style="background: black">3</div>
    <div style="background: green">4</div>
    <div style="background: yellow">5</div>
    <div style="background: red">6</div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
};
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

.container {
  width: 90%;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  /* grid-template-columns: repeat(3, 100px);
    === grid-template-columns: 100px 100px 100px;

    repeat(auto-fit, 100px);  不是固定3列

    repeat(auto-fit, minmax(100px, 1fr));
    minmax()函数定义的范围大于或等于min， 小于或等于max。
    因此，现在每列将至少为 100px。

     */
  grid-template-rows: 300px 300px;
  font-size: 20px;
  line-height: 300px;
  color: #fff;
}
.container div {
  text-align: center;
}
</style>
