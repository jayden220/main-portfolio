<template>

  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Serif+4:ital,opsz,wght@0,8..60,200..900;1,8..60,200..900&display=swap');

#app {
  font-family: "Source Serif", serif;
  /* font-weight: 400; */
  /* font-style: normal; */
  /* -webkit-font-smoothing: antialiased; */
  /* -moz-osx-font-smoothing: grayscale; */
  text-align: center;
  /* color: #2c3e50; */
}
::-webkit-scrollbar {
  width: 12px;
}
::-webkit-scrollbar-track {
  background: #ffffff; 
  
}
::-webkit-scrollbar-thumb {
  background: linear-gradient(90deg, #ffbc00, #ff0058); 
  border-radius: 6px; 
}
::-webkit-scrollbar-thumb:hover {
  background: #555555; 
}
/* For Firefox */
* {
  scrollbar-width: thin; 
  scrollbar-color: #000000 #ffffff; 
}
body{
  font-family: "Gilda Display", serif;
}
button{
  font-family: "Gilda Display", serif;
}

nav {
  /* padding: 30px; */
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  /* color: #42b983; */
}
</style>
