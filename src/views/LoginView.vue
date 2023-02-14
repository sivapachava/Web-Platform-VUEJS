<template>
  <div class="loginform"> 
    <div class="loginbox">
    <div class="fa fa-user-circle image-icon"></div>
    <h1>Login Here</h1>
               <form>
                   <p>Username</p>
                   <input type="text" name="" placeholder="Enter Username">                
                   <p>Password</p>
                   <input type="password" name="" placeholder="Enter password">
                   <div class="Button">                 
                   <input type="submit" name="" value="login">
                   </div>
                   <a href="">Forgot Your Password?</a><br>
                   <a href="">Don't have an account?</a>                            
               </form> 
           </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.loginform{
    width:100%;
    height:90vh;
    display: flex;
    margin-top: 10px;
    background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\main-vue-p\src\assets\backimage.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}
.loginbox{
    align-items: center;
    position: absolute;
    width:670px;
    height:430px;
    margin-left: 300px;
    background: hsl(180, 4%, 90%);
    box-sizing:border-box; 
    padding: 70px 30px;
    margin-top: 70px;   
}
.image-icon{
    width:70px;
    height:70px;
    border-radius:50%;
    position: absolute;
    left: 300px;
    top: 5px;
}
h1{
    margin:0;
    padding: 0 0 20px;
    text-align: center;
    font-size: 42px;
}
.loginbox p{
    margin:0;
    padding:0;
    font-weight: bold;
    font-size: 20px;
    margin-left: 90px;
    display: flex;
}
.loginbox input{
    width: 70%;
    margin-bottom: 20px;
}
.loginbox input[type="text"], input[type="password"]
{
    border: none;
    border-bottom: 1px solid rgb(28, 27, 27);
    background: transparent;
    height: 40px;
    font-size: 18px;
}
form .Button
{
    height: 25px;
    margin: 25px 170px;
    border-radius: 5px;
    padding: 0px 200px 0px 100px;
    width: 100%;
    
}
.loginbox input[type="submit"]
{
    border: none;
    width: 10%;
    background: rgb(26, 24, 24);
    height: 40px;
    font-size: 20px;
    text-align: center;
    outline:none;
    color:#fff;
    border-radius: 5px;
    display:flex;
    flex-wrap: wrap;
    padding: 0px 50px 0px 10px;
}
.loginbox input[type="submit"]:hover
{
    cursor: pointer;
    background: #aaa38d;
    color: #000;
    position: relative;
}
.loginbox a
{
    text-decoration: none;
    font-size: 15px;
    line-height: 20px;
    color: darkblue;
    padding-right: 300px;
}
.loginbox a:hover
{
    color: #db4227
}
</style>