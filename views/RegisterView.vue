<script setup>
import imgButton from '@/assets/images/backbutton.png'
import imgBirthday from '@/assets/images/birthday.gif'
</script>

<template>
  <body>
    <div class="container">
      <div class="row">
        <div class="col-2 col-md-5 col-lg-5 py-5 px-4">
          <RouterLink to="/Login"> <img :src="imgButton" width="55px" height="60px" /></RouterLink>
        </div>
        <div class="col-2 col-md-5 col-lg-6 py-1 px-5 mx-4">
          <div>
            <img :src="imgBirthday" height="150px" width="150px" />
          </div>
        </div>
      </div>
    </div>
    <div class="container py-2 px-4">
      <h1 class="">
        <center><b>Create Your Account</b></center>
      </h1>
      <span><center>Sign-up and create your account here</center></span> <br />

      <div class="mb-3">
        <i class="bi bi-person-fill pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>Name</b></label>
        <input
          type="Name"
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Enter your name"
        />
      </div>

      <div class="mb-3">
        <i class="bi bi-envelope-fill pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>E-mail Address</b></label>
        <input
          type="email"
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Enter your e-mail address"
        />
      </div>

      <div class="mb-3">
        <i class="bi bi-geo-alt-fill pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>Address</b></label>
        <input
          type="address"
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Enter your address"
        />
      </div>

      <div class="mb-3">
        <i class="bi bi-telephone-fill pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>Phone Number</b></label>
        <input
          type="phone number  "
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Enter your phone number"
        />
      </div>

      <div class="mb-3">
        <i class="bi bi-person-circle pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>Create Your Username</b></label>
        <input
          type="username"
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Enter your username"
        />
      </div>

      <div class="mb-3">
        <i class="bi bi-lock-fill pe-2"></i>
        <label for="exampleFormControlInput1" class="form-label"><b>Create Your Password</b></label>
        <input
          type="password"
          class="form-control"
          id="exampleFormControlInput1"
          placeholder="Consists of 8 characters"
        />
      </div>
      <br />
      <div class="form-check">
        <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault" />
        <label class="form-check-label" for="flexCheckDefault">
          I agree with the terms and conditions
        </label>
      </div>

      <div class="d-grid gap-2">
        <button class="btn" type="button">SIGN-UP</button>
      </div>

      <br />
      <p class="pt-2 text-center">
        Already have an account?
        <RouterLink class="link-opacity-100" to="/login"> <b>Sign in here</b></RouterLink>
      </p>
    </div>
  </body>
</template>

<style scoped>
.container p text {
  color: white;
}

body {
  background: linear-gradient(to left, orange 0%, orangered 100%);
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial,
    sans-serif;
}
span {
  color: aliceblue;
  font-size: small;
}
.form-check {
  color: aliceblue;
  font-size: small;
}
.btn {
  background-color: orangered;
  color: white;
  border-radius: 30px;
  border-color: orangered;
  font-size: medium;
  display: inline;
  height: 65px;
}
.btn:hover {
  color: white;
}
.form-control {
  border-radius: 20px;
  padding: 12px;
}
</style>
