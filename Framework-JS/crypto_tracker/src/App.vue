<template>
  <div class="container">
    <div class="tracker">
      <div class="trackerTop">
        <Title msg="CRYPTO TRACKER"/>
        <SearchInput name="search" text="Search..."/>
      </div>
      <div class="trackerList">
        
      </div>
    </div>
  </div>
</template>

<script>
import Title from './components/Title.vue';
import SearchInput from './components/input/SearchInput.vue';

export default {
  name: 'Tracker',
  components: {
    Title,
    SearchInput
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
