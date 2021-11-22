<template>
    <div class="select">
      <label for="description">Profession</label>
      <select name="work" id="workList">
        <option value="student">Etudiant</option>
        <option value="employee">Employé</option>
      </select>
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
