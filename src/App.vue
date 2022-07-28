<template>
  <nav>
    <router-link to="/">
      <img alt="home" src="../src/assets/home-white.svg" class="home">
    </router-link> |
    <router-link to="/tours">Tours</router-link> |
    <router-link to="/activities">Activities</router-link> |
     <router-link to="/about">About Us</router-link> 
  </nav>
  <router-view/>

</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.home{
  margin-bottom: -7px;
  max-width: 25px;
  

}
nav {
  margin-top: -12px;
  padding: 8px 12px 18px 12px;
  background-color: #42b983;
  color: #fff;
  
  font-size: 2em;
}

nav a {
  text-decoration: none;
  font-size: 16px;
  font-weight: bold;
  color: #fff;
  padding: 6px 13px;
  border-radius: 10px;
  border: #fff solid 2px;
}

nav a.router-link-exact-active {
  background-color: #fff;
  color: #42b983;
   font-size: 20px;
   margin-top: 50px;
}
nav a.router-link-exact-active.home {
  background-color: #fff;
  color: #42b983;
   font-size: 20px;
   margin-top: 50px;
  filter: invert(48%) sepia(79%) saturate(2476%) hue-rotate(86deg) brightness(118%) contrast(119%)
}
</style>
