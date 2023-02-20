<template>
  <div class="store">
    <div class="title1"> 
            <h1>Collections</h1>
            <h2>Explore our collection by theme, topic, century, and organisation. is a public library specializing in the field of Natural Sciences, and rich in an important heritage fund . Its activity is part of the general action of the Museum. This resource center of the institution in terms of documentation is intended both for the teams of the Museum and for the general public. It contributes to the dissemination of knowledge and provides its readers with updated scientific documentation enriched by regular acquisitions.</h2>
        </div>
        <div class="title2"> 
            <h1>Collections</h1>
            <h2>Explore our collection by theme, topic, century, and organisation. is a public library specializing in the field of Natural Sciences, and rich in an important heritage fund . Its activity is part of the general action of the Museum. This resource center of the institution in terms of documentation is intended both for the teams of the Museum and for the general public. It contributes to the dissemination of knowledge and provides its readers with updated scientific documentation enriched by regular acquisitions.</h2>
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

<style>
.store{
  margin-top: -15px;
  margin-left: 0px;
  background-color: rgb(247, 246, 245);
  height: 100vh;
}
.title1 h1{
  align-items: center;
  padding-top: 5px;
  margin-bottom: 10px;
  margin-left: 25px;
  font-size:35px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
  text-decoration: underline;
}
.title1 h2{
  align-items:flex-end;
  padding-top: 5px;
  margin-bottom: 10px;
  margin-left: 50px;
  font-size: 20px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif; 
  text-decoration:none;
}
.title2 h1{
  align-items: center;
  padding-top: 5px;
  margin-bottom: 10px;
  margin-left: 25px;
  font-size:35px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
  text-decoration: underline;
}
.title2 h2{
  align-items:flex-end;
  padding-top: 5px;
  margin-left: 50px;
  font-size: 20px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif; 
  text-decoration:none;
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