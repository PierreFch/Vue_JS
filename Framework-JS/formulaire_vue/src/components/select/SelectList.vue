<template>
    <label for="description">Profession</label>
    <select name="work" id="workList" v-model="selected">
      <option v-for="option in options" :key="option.text" v-bind:value="option.value">{{ option.text }}</option>
    </select>
</template>

<script>  
export default{
  data(){
    return{
      selected: '1',
      options: [
        {text: 'Etudiant', value: '1'},
        {text: 'Employé', value: '2'},
      ]
    }
  }
}
</script>

<style scoped>
  label{
    display: block;
  }
</style>