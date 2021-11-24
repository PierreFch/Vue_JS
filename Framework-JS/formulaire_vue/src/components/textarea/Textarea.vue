<template>
      <label for="description">{{label}}</label>
      <textarea name="description" id="description"></textarea>
</template>

<script>  
export default{
  name: 'Textarea',
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
