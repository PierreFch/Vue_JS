<template>
  <div class="hello">
    <h1>Hello world</h1>
    <div id="nameList">
        <ul class="list">
          <li v-for="item in items">{{ item }}</li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}

var nameList = new Vue({
  el: '#nameList',
  data: {
    items: [
      'Arthur',
      'Pierre',
      'Mathis',
      'Toto',
      'Tata',
    ]
  }
})

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

ul.list{
  display: flex;
  flex-direction: column;
}

ul.list li{
  margin: 10px 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
