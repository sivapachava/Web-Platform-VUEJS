<template>
  <div class="home">
    <div class="collectionform">
        <div class="title1"> 
    <h1>Museums of Information Technologies</h1>
    <h2>It aims to safeguard the contemporary scientific and technical heritage of Information Technology (IT) through the collections of computer museums</h2>
  </div>
    <form>
        <input type="text" placeholder="What you are looking for?">
        <button type="submit">search</button>
    </form>
</div>
  </div>
  <div class="title2"> 
    <h1>Explore</h1>
    <h2>Join with us to explore your Museum data and to represents an important part of the regional and national scientific and cultural heritage data</h2>
    </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    //HelloWorld
  }
}
</script>
<style scoped>
.home{
    width:100%;
    height:100vh;
    display: flex;
    margin-top: 10px;
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\main-vue-p\src\assets\backimage.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}
.title1 h1{
    font-size: 45px;
    font-weight: bold;
    font-style: inherit;
    display: flex;
    margin-top: 100px;
    margin-left: 20px;
    color: rgb(13, 13, 14);
    align-items: center;
    justify-content: center;
}
.title1 h2{
    font-size:25px;
    font-weight: bold;
    font-style: inherit;
    margin-left: 20px;
    display: flex;
    color: rgb(13, 13, 14);
    align-items: center;
    justify-content: center;
}
.collectionform form {
    background: #fff;
    width:600px;
    height:40px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 300px;
    margin-top: 70px;
}
.collectionform form input{
    flex:1;
    border:none;
    outline: none;
    font-size: medium;
}
.collectionform form button{
    background: rgb(11, 11, 11);
    padding: 10px 50px;
    border:none;
    outline: none;
    color: #fff;
    letter-spacing: 1px;
    cursor: pointer;
    height: 40px;
    font-size: medium;
    font-weight: bold;
}
.title2 h1{
    text-decoration:underline;
    margin-top: 50px;
}
.title2 h2{
    text-decoration: none;
    text-decoration-line: none;
    margin-top: 20px;

}
</style>
