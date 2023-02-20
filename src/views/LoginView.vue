<template>
  <ForgotPasw />
  <div class="login-container">  
      <div>
    <form class="login-form" @submit.prevent="login">
      <div class="fa fa-user-circle image-icon"></div>
      <h2>Login Here</h2>
      <div class="form-group">
        <label for="username">Username</label>
        <input type="text" id="username" placeholder="Enter Your User Name" v-model="username" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <div class="password-container">
          <input id="password" :type="showPassword ? 'text' : 'password'"  v-model="password" placeholder="Enter Your Password"/>
          <span class="toggle-password" @click="toggleShowPassword">
          <i class="fa" :class="showPassword ? 'fa-eye-slash' : 'fa-eye'"></i>
        </span>
        </div>
      </div>
      <div class="form-group">
        <button type="submit">Login</button>
      </div>
      <div class="login-links">
      <router-link to="/forgot-password">Forgot Your Password?</router-link>
      <span> | </span>
      <router-link to="/signup">Don't have an account?</router-link>
    </div>
    </form>
  </div>
</div>
</template>

<script>
import axios from "axios";
import ForgotPasw from "./ForgotPasw.vue"
export default {
  path: '/forgot-password',
  name: 'forgotPassword',
  component: ForgotPasw,
  data() {
    return {
      username: '',
      password: '',
      showPassword: false,
    }
  },
  methods: {
    login() {
  // Make an API call to authenticate the user
  // You can use axios or any other library to make the API call
  axios.post('/api/login', {
    username: this.username,
    password: this.password
  })
    // Navigate to the home page upon successful login
    this.$router.push('/')
  
  .catch(error => {
    console.log(error)
    alert('Login failed')
  });
},
toggleShowPassword() {
        this.showPassword = !this.showPassword;
      },
  }
}
</script>

<style scoped>

.login-container {
  display: flex;
  flex-direction: column;
  margin-top:5px;
  align-items: center;
  background-size: cover;
  width:100%;
  height:90vh;
  background-repeat: no-repeat;
  background-image: url("C:\Users\Siva Ratnam Pachava\OneDrive\Desktop\internship-project-m2\Web-Platform-VUEJS\src\assets\backimage.jpg");
}

.login-form {
  width: 500px;
  height: 380px;
  margin-top: 70px;
  margin-left: 50px;
  padding: 20px;
  background-color: #f0f0f0;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}
 .image-icon{
    width:70px;
    height:70px;
    border-radius:50%;
    position: absolute;
    left: 620px;
    top: 170px;
}

.login-form h2 {
  text-align: center;
  margin-bottom: 20px;
  margin-top: 70px;
}

.form-group {
  margin-bottom: 20px;
  margin-left: 25px;
}

label {
  font-weight: bold;
  margin-bottom: 10px;
  font-size: 18px;
  margin-left: -380px;
}

input[type="text"],
input[type="password"] {
  display: block;
  width: 90%;
  padding: 10px;
  border-radius: 5px;
  border: none;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
}
.password-container {
    display: flex;
    align-items: center;
  }
.fa-eye{
  cursor: pointer;
  margin-left: -30px;
}
button[type="submit"] {
  display: block;
  width: 95%;
  padding: 10px;
  border-radius: 5px;
  border: none;
  background-color: #3f51b5;
  color: #fff;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.2s;
  margin-bottom: 35px;
}

button[type="submit"]:hover {
  background-color: #2c387e;
}

.login-links {
  margin-top: 20px;
  font-size: 14px;
}

.login-links a,
.login-links router-link {
  text-decoration: none;
  color: #3f51b5;
  font-weight: bold;
}

.login-links a:hover,
.login-links router-link:hover {
  text-decoration: underline;
}
</style>