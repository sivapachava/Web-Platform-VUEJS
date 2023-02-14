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
</template>

<script>
export default {
  
}
</script>

<style scoped>
.collect{
  margin-left: 0px;
  background-color: rgb(195, 194, 192);
  margin-top: 10px;
}
.title1{
  display: flex;
  align-items: center;
  padding-top: 0px;
  padding-left: 10px;
  font-size:15px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif;
}
.title1 h2{
  margin-top: 100px;
  margin-left: -160px;
  font-size: 20px;
  font-weight: bold;
  font-family: "Open Sans", sans-serif; 
}
.right-header-content h1{
  display: flex;
  align-items: center;
  margin-top: 50px;
  margin-left: 10px;
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
    background-image: url('C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\main-vue-p\src\assets\artlogo.jpg');
}
.image-2{
    background-image: url('C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\main-vue-p\src\assets\artlogo.jpg');
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
</style>
