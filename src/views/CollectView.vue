<template>
  <div class="collect">
    <div class="title1"> 
    <h1>Collections</h1>
    <h2>Explore our collection by theme, topic, century, and organisation</h2>
  </div>
  <div class="right-header-content">
        <h1>Themes</h1>
      </div> 
        <section class="container">
        <div class="card">
            <h2>Company</h2>
            <p>Get to know us and meet the people behind Musicca.</p>
            <div class="card-image image-1"></div>
        </div>
        <div class="card">
            <h2>Mission</h2>
            <p>Read our mission statement and learn more about our goals.</p>
            <div class="card-image image-2"></div>
        </div>
        <div class="card">
            <h2>Mission</h2>
            <p>Read our mission statement and learn more about our goals.</p>
            <div class="card-image image-2"></div>
        </div>
        <div class="card">
            <h2>Mission</h2>
            <p>Read our mission statement and learn more about our goals.</p>
            <div class="card-image image-2"></div>
        </div>
    </section>
    <div class="Button1">                
                <input type="Submit" value="Show More Themes">               
    </div>
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
export default {
  
}
</script>

<style scoped>
.collect{
  margin-left: 0px;
  background-color: rgb(195, 194, 192);
  margin-top: 0px;
}
.title1 h1{
  display: flex;
  align-items: center;
  padding-top: 5px;
  padding-left: 10px;
  font-size: 35px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
  margin-left: 30px;
}
.title1 h2{
  display: flex;
  align-items: center;
  margin-top: 10px;
  margin-left: 25px;
  font-size: 20px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
}
.right-header-content h1{
  display: flex;
  align-items: center;
  margin-top: 50px;
  margin-left: 50px;
  font-size:30px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
  color:rgb(12, 12, 12);
}
.container{
    display: flex;
    justify-content: center;
    margin-right: 40px;
}
.card{
    background: rgb(244, 244, 244);
    width: 270px;
    height: 250px;
    margin: 10px;
}
.card h2{
    padding: 5px;
}
.card p{
    padding: 5px
}
.card-image{
    background-color: rgb(228, 235, 235);
    height: 170px;
}
.image-1{
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\internship-project-m2\Web-Platform-VUEJS\src\assets\artlogo.jpg");
}
.image-2{
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\internship-project-m2\Web-Platform-VUEJS\src\assets\artlogo.jpg");
}
.Button1
{
    align-items: center;
    height: 25px;
    margin-top: 60px;
    border-radius: 10px;
    width:550px;
    padding: 20px;
    margin-left: -150px;
   
}
.Button1 input[type="submit"]
{
    border: none;
    width: 40%;
    background: rgb(239, 217, 217);
    height: 40px;
    font-size: 20px;
    text-align: center;
    outline:none;
    color:#000;
    font-weight: bold;
    border-radius: 10px;
    flex-wrap: wrap;
    padding: 0px 10px 0px 10px;
    align-items: center;
    font-family: sans-serif;
}
.Button1 input[type="submit"]:hover
{
    cursor: pointer;
    background: #d2c7f1;
    color: rgb(21, 20, 20);
    position: relative;
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
