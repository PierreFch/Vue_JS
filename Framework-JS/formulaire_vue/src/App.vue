<template>
<div class="image">
  <img alt="Vue logo" src="./assets/logo.png">
</div>
  <Title title="Formulaire de contact"/>
  <form id="contactForm">
    <TextInput />
    <DateInput />
    <TextArea />
    <SelectList />
    <RadioInput />
    <CheckInput />
    <ValidationSubmit />
    <ResetSubmit />
    <ErrorMessage />
    <SuccessMessage />
  </form>
</template>

<script>  
  import Title from'./components/title/Title.vue';
  import TextInput from'./components/input/TextInput.vue';
  import DateInput from './components/input/DateInput.vue';
  import TextArea from './components/input/Textarea.vue';
  import SelectList from './components/select/SelectList.vue';
  import RadioInput from './components/input/RadioInput.vue';
  import CheckInput from './components/input/CheckInput.vue';
  import ValidationSubmit from './components/submit/ValidationSubmit.vue';
  import ResetSubmit from './components/submit/ResetSubmit.vue';
  import ErrorMessage from './components/message/ErrorMessage.vue';
  import SuccessMessage from './components/message/SuccessMessage.vue';
  export default {
  name: 'App',
    components: {
      Title,
      TextInput,
      DateInput,
      TextArea,
      SelectList,
      RadioInput,
      CheckInput,
      ValidationSubmit,
      ResetSubmit,
      ErrorMessage,
      SuccessMessage
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  text-align: center;
}
form#contactForm{
  text-align: left;
  width: 40%;
  margin: auto;
}
form#contactForm div{
  margin: 10px;
}
div.text:nth-of-type(1){
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
label{
  padding-right: 5px;
}
</style>
