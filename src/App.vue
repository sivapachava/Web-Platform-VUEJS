<template>
  <div class="menu-bar">
  <div class="title">MuseumIT</div>
  <nav>
    <router-link to="/" class="button-left">Home</router-link>
    <router-link to="/collections" class="button-left">Collections</router-link>
    <router-link to="/stories" class="button-left">Stories</router-link>
    <router-link to="/login" class="button-left">LogIn</router-link>
    <router-link to="/signup" class="button-left">SignUp</router-link>
  </nav>
  <i class="fa fa-search search-icon"></i>
</div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #101111;
}
.menu-bar{
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 70px;
  background-color: rgb(243, 225, 28);
  width: 100%;
}
.title{
  padding-left: 200px;
  font-family: sans-serif;
  font-size: xx-large;
  font-weight:bold;
  margin-right: 200px;
}
nav {
  padding: 20px;
  margin-right:100px;
  display: flex;
  align-items: center;
  justify-content: space-between;

}
.button-left {
  font-family: "Open Sans", sans-serif;
  font-size: 14px;
  color: black;
  border: none;
  border-radius: 20px;
  padding-top: 8px;
  padding-right: 15px;
  padding-left: 15px;
  padding-bottom: 8px;
  font-weight: 600;
  margin-right: 4px;
  text-decoration: none;
}
.button-left:hover {
  background-color: rgb(194, 131, 131);
}
.search-icon{
  align-items: center;
  margin-top: 10px;
  margin-right: 50px;
  cursor: pointer;
}
nav a.router-link-exact-active {
  font-family: "Open Sans", sans-serif;
  font-size: 14px;
  color: black;
  border: none;
  border-radius: 20px;
  padding-top: 8px;
  padding-right: 15px;
  padding-left: 15px;
  padding-bottom: 8px;
  font-weight: 600;
  margin-right: 4px;
  text-decoration: none;
  background-color: #42b983;
}

</style>
