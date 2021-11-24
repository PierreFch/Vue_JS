<template>
<span v-for="gender in genders" :key="gender.text">
    <input type="radio" v-bind:id="gender.nameId" v-bind:name="name" v-bind:value="gender.value">
    <label v-bind:for="gender.nameId" >{{gender.label}}</label>
</span>
</template>

<script>  
export default{
  name: 'RadioInput',
  props: {
    name: String,
    label: String,
    value: String,
    nameId: String
  },
  data(){
    return{
      genders: [
        {label: 'Homme', value: 'man', nameId: 'man'},
        {label: 'Femme', value: 'woman', nameId: 'woman'},
      ]
    }
  }
}
</script>
<style>

</style>
