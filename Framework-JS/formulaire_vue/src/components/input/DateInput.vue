<template>
    <label for="bornDate">{{label}}</label>
    <input type="date" id="bornDate" name="bornDate" value="bornDate" >
</template>

<script>  
export default{
  name: 'DateInput',
  props: {
    label: String
  }
}
</script>

<style scoped>
  label{
    display: block;
  }
</style>
