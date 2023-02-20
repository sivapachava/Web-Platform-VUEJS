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

    <div class="foot-container">
      <nav class="footer-nav">
        <ul>
          <li><a href="#">Contact Us</a></li>
          <li><a href="#">Privacy and Policy</a></li>
          <li><a href="#">Cookies</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Become a data partner</a></li>
          <li><a href="#">Conditions</a></li>
        </ul>
      </nav>
      <div class="footer-social">
        <ul>
          <li><a href="#"><i class="fab fa-instagram" color="white"></i></a></li>
          <li><a href="#"><i class="fab fa-twitter" color="white"></i></a></li>
          <li><a href="#"><i class="fab fa-linkedin" color="white"></i></a></li>
        </ul>
      </div>
      <div class="footer-copy">
        <p>&copy; 2023 Our Company. All rights reserved.</p>
      </div>
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
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\internship-project-m2\Web-Platform-VUEJS\src\assets\backimage.jpg");
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
    margin-left: 5px;
}
.title2 h2{
    text-decoration: none;
    text-decoration-line: none;
    margin-top: 20px;
    font-size: 20px;

}




.foot-container {
  height: 150px;
  width: 100%;
  background-color: rgb(78, 75, 75);
  margin-top: 120px;
}

.footer-nav ul {
  display: flex;
  padding-right: 20px;
  padding-left: 20px;
  list-style: none;
  margin-top: 0px;
}

.footer-nav li {
  margin-right: 40px;
  margin-left: 40px;
  margin-top: 10px;
}

.footer-nav a {
  color: rgb(243, 240, 240);
  text-decoration: none;
  font-family: sans-serif;
}
.footer-nav a:hover {
  color: rgb(243, 240, 240);
  text-decoration:underline;

}
.footer-social ul {
  list-style: none;
  display: flex;
  margin-left: 30px;
}

.footer-social li {
  display: flex;
  margin-right: 30px;
}

.footer-social i {
  font-size: 24px;
  color: rgb(243, 240, 240);
}

.footer-copy {
  font-size: 12px;
  color: rgb(243, 240, 240);
  margin-left: 100px;
}
</style>
