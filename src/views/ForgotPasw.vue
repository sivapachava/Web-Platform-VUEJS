<template>
  <div class="container">
    <div class="forgot-password">
      <h2>Forgot Password?</h2>
      <form @submit.prevent="resetPassword">
        <div class="form-group">
          <label for="newPassword">New Password</label>
          <div class="password-input">
            <input id="password" :type="showPassword ? 'text' : 'password'" v-model="password" placeholder="Enter new password"/>
            <span class="toggle-password" @click="togglePasswordVisibility">
            <i :class="showPassword ? 'fa fa-eye-slash ' : 'fa fa-eye'"></i>
          </span>
          </div>
        </div>
        <div class="form-group">
          <label for="confirmPassword">Confirm Password</label>
          <div class="password-input">
            <input id="confirmPassword" :type="showPassword ? 'text' : 'password'" v-model="confirmPassword" placeholder="Re-enter new password"/>
            <span class="toggle-password" @click="togglePasswordVisibility">
            <i :class="showPassword ? 'fa fa-eye-slash ' : 'fa fa-eye'"></i>
            </span>
          </div>
        </div>
        <div class="form-group">
          <button type="submit" @click.prevent="handleSubmit">Reset Password</button>
        </div>
        <div class="login-links">
          <router-link to="/login">Back to Login</router-link>
        </div>
      </form>
    </div>
  </div>
  </template>
  
  <script>
  import axios from "axios";
  export default {
    data() {
      return {
        newPassword: "",
        confirmPassword: "",
        showPassword: false,
      };
    },
    methods: {
      resetPassword() {
        if (this.newPassword !== this.confirmPassword) {
          alert("Passwords do not match");
          return;
        }
        // Make an API call to reset the user's password
        // You can use axios or any other library to make the API call
        axios
          .post("/api/reset-password", {
            newPassword: this.newPassword,
          })
          .then(() => {
            // Redirect to the login page upon successful password reset
            this.$router.push("/login");
          })
          .catch((error) => {
            console.log(error);
            alert("Password reset failed");
          });
      },

      togglePasswordVisibility() {
      this.showPassword = !this.showPassword;
    },
    handleSubmit() {
      // Submit the form data here
      console.log('Form submitted');
    },

    },
  }
  </script>
  
  <style scoped>
 .container{
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
  .forgot-password {
    width: 500px;
    margin-top: 70px;
    margin-left: 50px;
    padding: 20px;
    background-color: #f0f0f0;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  }
  
  .forgot-password h2 {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .form-group {
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
  }
  .form-group label {
    font-weight: bold;
    margin-bottom: 10px;
    font-size: 18px;
    margin-right: 300px;
  }
.password-input {
  position: relative;
  display: flex;
  width: 100%;
}
input {
  width: 100%;
  padding: 10px;
  border-radius: 5px;
  border: none;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
}
.fa-eye{
  margin-left: -25px; 
  margin-top: 10px;
  cursor: pointer;
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
  margin-bottom: 25px;
  margin-left: 15px;
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