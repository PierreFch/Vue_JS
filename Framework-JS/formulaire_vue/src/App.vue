<template>
<div class="image">
  <img alt="Vue logo" src="./assets/logo.png">
</div>
  <Title title="Formulaire de contact"/>
  <form id="contactForm">
    <div class="text">
      <TextInput />
    </div>
    <div class="radio">
      <RadioInput />
    </div>
    <div class="date">
      <DateInput />
    </div>
    <div class="textarea">
      <Textarea />
    </div>
    <div class="select">
      <SelectList />
    </div>
    <CheckInput />
    <div class="submit">
        <ResetSubmit />
        <ValidationSubmit />
    </div>
    <div class="message">
        <ErrorMessage />
        <SuccessMessage />
    </div>
  </form>
</template>

<script>  
  import Title from'./components/title/Title.vue';
  import TextInput from'./components/input/TextInput.vue';
  import RadioInput from './components/input/RadioInput.vue';
  import DateInput from './components/input/DateInput.vue';
  import Textarea from './components/textarea/Textarea.vue';
  import SelectList from './components/select/SelectList.vue';
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
      RadioInput,
      DateInput,
      Textarea,
      SelectList,
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
form#contactForm > div{
  margin: 10px;
}
div.text:nth-of-type(1){
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
label{
  padding: 0 5px 5px 0;
  font-size: 1.1em;
}
input, textarea{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  font-size: 1em;
  min-height: 25px;
  width: 100%;
}
select{
  border: 1px solid #000;
  background: #35495E;
  color: #FFF;
  padding: 5px 20px;
  font-size: 1em;
  cursor: pointer;
}
input[type="radio"], input[type="checkbox"]{
  width: auto;
}
textarea{
  resize: none;
}
div.radio span, div.check span{
  font-size: 1.1em;
}
div.radio label, div.check label{
  font-size: 1em;
  padding-bottom: 0;
  cursor: pointer;
}
div.radio input, div.check input{
  min-height: auto;
}
div.submit{
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  padding: 20px 0;
}
</style>
