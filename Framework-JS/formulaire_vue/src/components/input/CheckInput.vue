<template>
<span>{{label}}</span>
  <div v-for="job in jobs" :key="job.text" class="job">
    <input type="checkbox" v-bind:id="job.nameId" v-bind:name="job.nameId" v-bind:value="job.value"> 
    <label v-bind:for="job.nameId">{{job.text}}</label>
  </div>
</template>

<script>  
export default{
  name: 'CheckInput',
  props: {
    name: String,
    label: String,
    value: String,
    nameId: String
  },
  data(){
    return{
      jobs: [
        {text: 'Marketing', value: 'Marketing', nameId: 'marketing'},
        {text: 'Développement', value: 'developpement', nameId: 'developpement'},
        {text: 'Webdesign', value: 'webdesign', nameId: 'webdesign'},
        {text: 'Product Managment', value: 'productManagment', nameId: 'productManagment'}
      ]
    }
  }
}
</script>

<style>

</style>
