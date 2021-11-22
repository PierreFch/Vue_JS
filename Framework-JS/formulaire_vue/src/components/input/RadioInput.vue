<template>
    <div class="radio">
      <span>Sexe :</span>
      <label for="man">Homme</label>
      <input type="radio" id="man" name="drone" value="man">
      <label for="woman">Femme</label>
      <input type="radio" id="woman" name="drone" value="woman">
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

<style>

</style>
