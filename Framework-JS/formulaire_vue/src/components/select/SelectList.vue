<template>
    <label for="workList">{{label}}</label>
    <select name="work" id="workList" v-model="selected">
      <option v-for="option in options" :key="option.text" v-bind:value="option.value">{{ option.text }}</option>
    </select>
</template>

<script>  
export default{
  name: 'SelectList',
  props: {
    label: String
  },
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
  select{
  border: 1px solid #000;
  background: #35495E;
  color: #FFF;
  padding: 5px 20px;
  font-size: 1em;
  cursor: pointer;
  width: 100%;
}
</style>