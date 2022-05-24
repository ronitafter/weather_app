<template>
<div id="app">
  <main>
    <div class="search-box">
      <input type="text" name="" id="" 
      class="search-bar" placeholder="Search..."/>
    </div>
    <div class="weather-wrap">
      <div class="location-box">
        <div class="location">Tel Aviv, Israel</div>
        <div class="date">Tuesday 24 May 2022</div>
      </div>
      <div class="weather-box">
        <div class="temp">15ºc</div>
        <div class="weather">Rain</div>
      </div>
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

.search-box .search-bar{
  display:block;
  width: 100%;
  padding: 15px;
  color: #313131;
  font-size: 20px;
  appearance: none;
  border: none;
  outline: none;
  background: none;
  box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 0px 16px 0px 16px;
  transition: 0.4s;
}

.search-box .search-bar:focus {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 16px 0px 16px 0px;
}

.location-box .location{ 
  color: #fff;
  font-size: 25px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0, 0, 0, 0.25);

}
</style>
