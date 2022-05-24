<template>
<div id="app">
  <main>
    <div class="search-box">
      <input type="text" name="" id="" 
      class="search-bar" placeholder="Search..."/>
    </div>
  </main>
</div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      api_key: 'a58280c47755ba696d4317a40a156d56'
    }
  }

}
</script>
<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  font-family: sans-serif, 'Times New Roman', Times, serif;
}
#app{
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}
main{
  min-height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
}
.search-box{
  width: 100%;
  margin-bottom: 30px;
}
</style>
