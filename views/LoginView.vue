<script setup>
import imgLogo from '@/assets/images/tiny taster logo.png'
</script>

<template>
  <body class="bg-body-tertiary pb-5">
    <br />
    <br />
    <br />
    <br />
    <div class="container">
      <div class="card text-bg-warning bg-opacity-25">
        <div class="card-body">
          <div class="row">
            <!--image of header-->
            <div class="col-md-8 col-lg-5 py-5 px-2 text-center">
              <img :src="imgLogo" class="rounded-5" height="320px" width="320" />
            </div>
            <!-- end of image-->

            <!--username-->
            <div class="  ">
              <i class="bi bi-person-circle pe-2"></i>
              <label for="exampleFormControlInput1" class="form-label"><b>Username</b></label>
              <input
                type="username"
                class="form-control"
                id="exampleFormControlInput1"
                placeholder="Enter your username"
              />

              <!--end of username-->
              <br />
              <!--password-->
              <i class="bi bi-lock-fill pe-2"></i>
              <label for="exampleFormControlInput1" class="form-label"><b>Password</b></label>
              <input
                type="password"
                class="form-control"
                id="exampleFormControlInput1"
                placeholder="Enter your password"
              />

              <!--end of password-->
              <br />

              <!--button-->
              <div class="d-grid gap-2">
                <button class="btn btn-primary" type="button">LOG IN</button>
              </div>
              <!--end of button-->

              <p>
                <a
                  href="#"
                  class="link-dark link-offset-2 link-underline-opacity-25 link-underline-opacity-100-hover"
                  ><center>Forgot Password?</center></a
                >
              </p>

              <br />

              <p>
                <center>
                  Don't have an account?
                  <RouterLink to="/register"> <b> Sign Up </b></RouterLink>
                </center>
              </p>
            </div>
          </div>
        </div>
      </div>
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
