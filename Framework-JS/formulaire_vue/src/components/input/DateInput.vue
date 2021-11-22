<template>
    <div class="date">
      <label for="bornDate">Date de naissance</label>
      <input type="date" id="bornDate" name="bornDate" value="bornDate" >
    </div>
</template>

<script>  
  export default {
  name: 'title',
  props: {
    title: String
  }
}
</script>

<style scoped>
  label{
    display: block;
  }
</style>
