<template>
  <div class="signupform">
    <form class="content" @submit.prevent="register">
      <h2>Create an Account Here!</h2>
      <div class="user-details">
      <div class="input-box">
        <label class="deatils" for="firstName">First Name</label>
        <input type="text" id="firstName" placeholder="Enter Your First Name" v-model="firstName" required>
      </div>
      <div class="input-box">
        <label class="deatils" for="lastName">Last Name</label>
        <input type="text" id="lastName" placeholder="Enter Your Last Name" v-model="lastName" required>
      </div>
      <div class="input-box">
        <label class="deatils" for="phoneNumber">Phone Number</label>
        <input type="text" id="phoneNumber" placeholder="Enter Your Phone Number" v-model="phoneNumber" required>
      </div>
      <div class="input-box">
        <label class="deatils" for="email">Email</label>
        <input type="email" id="email" placeholder="Enter Your EmailID" v-model="email" required>
      </div>
      <div class="input-box">
        <label class="deatils" for="password">Password</label>
        <input type="password" id="password" placeholder="Enter Your Password" v-model="password" required>
      </div>
      <div class="input-box">
        <label class="deatils" for="confirmPassword">Confirm Password</label>
        <input type="password" id="confirmPassword" placeholder="ReEnter Your Password" v-model="confirmPassword" required>
      </div>
      <div>
        <button type="submit">Register</button>
      </div>
    </div>
    </form>
    </div>
  </template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      firstName: '',
      lastName: '',
      phoneNumber: '',
      email: '',
      password: '',
      confirmPassword: ''
    }
  },
  methods: {
    register() {
      if (this.password !== this.confirmPassword) {
        alert('Passwords do not match')
        return
      }
      // Make an API call to register the user
      // You can use axios or any other library to make the API call
      axios.post('/api/register', {
        firstName: this.firstName,
        lastName: this.lastName,
        phoneNumber: this.phoneNumber,
        email: this.email,
        password: this.password
      })
        // Redirect to the login page upon successful registration
        this.$router.push('/login')
      
      .catch(error => {
        console.log(error)
        alert('Registration failed')
      })
    }
  }
}
</script>

<style scoped>

.signupform {
  background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\internship-project-m2\Web-Platform-VUEJS\src\assets\backimage.jpg");
  margin-top: 5px;
  background-size: cover;
  width: 100%;
  height: 100vh;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.content {
  width: 700px;
  height: 400px;
  margin-top: 70px;
  padding: 20px;
  background-color: #f0f0f0;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

.content h2 {
  text-align: center;
  margin-bottom: 30px;
}

.content .user-details
{
    display: flex;
    flex-wrap: wrap;
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
    font-size: 10px;
    color:#000;
    font-style:inherit;
}
label{
  font-size: 15px;
  font-weight: bold;
  font-family: sans-serif;
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
    margin-bottom: 25px;
    border-bottom-width: 2px;
    transition: all 0.3s ease;
}

button[type="submit"] {
  display: block;
  width: 100%;
  padding: 10px;
  border-radius: 5px;
  border: none;
  background-color: #3f51b5;
  color: #fff;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.2s;
  margin-left: 200px;
  margin-top:30px;
}

button[type="submit"]:hover {
  background-color: #2c387e;
}
</style>