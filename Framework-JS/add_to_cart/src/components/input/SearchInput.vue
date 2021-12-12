<template>
  <div class="search">
    <input type="search" v-bind:id="name" v-bind:name="name" v-bind:placeholder="text"/>
  </div>
</template>

<script>
export default {
  name: 'SearchInput',
  props: {
    name: String,
    text: String
  }
}
</script>

<style scoped>
input{
    background: transparent;
    border: 1px solid #FFF;
    width: 25%;
    min-height: 45px;
    color: #FFF;
    border-radius: 10px;
    padding: 5px 10px;
}
div.search{
    text-align: center;
}
</style>