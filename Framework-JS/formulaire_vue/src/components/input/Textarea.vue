<template>
    <div class="textarea">
        <label for="description">Description</label>
        <textarea name="description" id="description"></textarea>
    </div>
</template>

<script>  
  export default {
  name: 'title',
  props: {
    label: String,
    textarea: String,
  }
}
</script>

<style scoped>
  label{
    display: block;
  }
</style>
