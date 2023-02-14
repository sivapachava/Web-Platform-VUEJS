<template>
  <div class ="signupform">
    <div class ="content"> 
    <h1 class="title1">Create an Account Here!</h1>
            <form action="#">
                <div class="user-details">
                <div class="input-box">
                <span class="detais">Fullname</span>               
                    <input type="text" name="" placeholder="Enter Your Fullname">
                   </div> 
                <div class="input-box">
                <span class="detais">Username</span>               
                    <input type="text" name="" placeholder="Enter Your Username">
                    </div>
                <div class="input-box">
                <span class="detais">Email ID</span>               
                    <input type="text" name="" placeholder="Enter Your Email ID">
                    </div>
                <div class="input-box">
                <span class="detais">Phone Number</span>               
                    <input type="text" pattern="[0-9] {10}"  name="" placeholder="Enter Your PhoneNumber">
                    </div>
                <div class="input-box">
                <span class="detais">Password</span>               
                    <input type="password" name="" placeholder="Enter Your Password">
                    </div>
                <div class="input-box">
                <span class="detais">Confirm Password</span>               
                    <input type="password" name="" placeholder="Confirm Your Password">
                    </div> 
                </div>                                 
                <div class="Country-Details">
                    <input type="radio" name="Country" id="dot-1">
                    <input type="radio" name="Country" id="dot-2">
                    <input type="radio" name="Country" id="dot-3">
                <span class="Country-Title">Coutry</span>
                    <div class="category">
                    <label for="dot-1">
                    <span class="dot one"></span>
                    <span class="Country">France</span>
                    </label>
                    <label for="dot-2">
                    <span class="dot two"></span>
                    <span class="Country">Italy</span>
                    </label>
                    <label for="dot-3">
                    <span class="dot three"></span>
                    <span class="Country">Other</span>
                    </label>
                </div>
                </div>
                <div class="Button">                
                <input type="Submit" value="Register">               
                </div>                                          
            </form>
  </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.signupform{
    width:100%;
    height:90vh;
    display: flex;
    margin-top: 10px;
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\main-vue-p\src\assets\backimage.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}
.content {
    width: 800px;
    height: 400px;
    margin-top: 50px;
    margin-right: auto;
    margin-left: auto;
    border-radius: 5px;
    background-color: rgb(242, 224, 224);
    padding-top: 20px;
    padding-bottom: 20px;
    padding-left: 50px;
    padding-right: 0px;
    font-family: sans-serif;
    
}
.title1{ 
    text-decoration-line: underline;
    margin-left: 0px;
    margin-top: 5px;
}
.content .user-details
{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-content: center; 
}
form .user-details .input-box
{
    width:  calc(100% / 2 - 20px);
}
.user-details .input-box .detais
{
    display: black;
    font-weight: bold;
    margin-bottom: 25px;
    font-size: 12px;
    color:#000;
    margin-right: 250px;
}
.user-details .input-box input
{
    height: 25px;
    width: 85%;
    outline: none;
    border-radius: 5px;
    border: 1px;
    padding-left: 15px;
    font-size: 12px;
    margin-bottom: 15px;
    border-bottom-width: 2px;
    transition: all 0.3s ease;
}
form .Country-Details .Country-Title
{
    font-size: 15px;
    font-weight:bold;
    margin-right:650px;
}
form .Country-Details .category
{
    display: flex;
    width: 80%;
    margin: 14px 0;
    justify-content: space-between;
}
.Country-Details .category label
{
    display: flex;
    align-items: center;
    margin-left:50px;
}
.Country-Details .category .dot
{
    height: 10px;
    width: 10px;
    background:rgb(235, 189, 189);
    border-radius: 50%;
    margin-right: 10px;
    border:5px solid transparent;
    transition: all 0.3s ease;
}
#dot-1:checked ~ .category label .one,
#dot-2:checked ~ .category label .two,
#dot-3:checked ~ .category label .three{
    border-color: rgb(42, 23, 188);
    background: rgb(172, 15, 15);
}
form input[type="radio"]
{
    display: none;
}
form .Button
{
    align-items: center;
    height: 20px;
    margin: 45px 155px;
    border-radius: 10px;
    padding: 0px 200px 0px 150px;
}
form .Button input[type="submit"]
{
    border: none;
    width: 40%;
    background: rgb(173, 123, 123);
    height: 40px;
    font-size: 15px;
    font-weight: bold;
    text-align: center;
    outline:none;
    color:#000;
    border-radius: 20px;
    display:flex;
    flex-wrap: wrap;
    padding: 0px 100px 0px 40px;
    font-family: sans-serif;
}
form .Button input[type="submit"]:hover
{
    cursor: pointer;
    background: #9281c2;
    color: #fff;
    position: relative;
}
</style>