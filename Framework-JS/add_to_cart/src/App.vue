<template>
  <div class="container">
  <Title msg="Ma boutique en ligne"/>
    <div class="content">
    
    </div>
  </div>
</template>

<script>
import Title from './components/Title.vue';

export default {
  name: 'App',
  components: {
    Title,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
body{
  background: #1A1A1C;
  color: #FFF;
  font-family: 'Montserrat', sans-serif;
  font-size: 1em;
  margin-top: 20px;
}
div.container{
  max-width: 1200px;
  padding: 0 20px;
  margin: auto;
}
input{
    font-family: 'Montserrat', sans-serif;
}
</style>
