<template>
    <div class="check">
      <span>Compétences :</span>
      <div class="checkbox">
        <label for="marketing">Marketing</label>
        <input type="checkbox" id="marketing" value="marketing">
      </div>
      <div class="checkbox">
        <label for="developpement">Développement</label>
        <input type="checkbox" id="developpement" value="developpement">
      </div>
      <div class="checkbox">
        <label for="webdesign">Webdesign</label>
        <input type="checkbox" id="webdesign" value="webdesign">
      </div>
      <div class="checkbox">
        <label for="productManagment">Product managment</label>
        <input type="checkbox" id="productManagment" value="productManagment">
      </div>
    </div>
</template>

<script>  
  export default {
  name: 'title',
  props: {
    label: String,
    input: String,
  }
}
</script>

<style>

</style>
