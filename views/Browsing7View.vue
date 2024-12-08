<script setup>
import img1 from '@/assets/images/Minecraft 1.png'
import img2 from '@/assets/images/Minecraft 2.png'
import img3 from '@/assets/images/Roblox.png'
import img4 from '@/assets/images/Biker.png'
import img5 from '@/assets/images/Moto.png'
import img6 from '@/assets/images/ML.png'

import imgLogo from '@/assets/images/tiny taster logo.png'
import imgGif from '@/assets/images/gif 2.gif'
import imgButton from '@/assets/images/backbutton.png'
</script>

<template>
  <div class="bg-warning-subtle">
    <div class="header">
      <div class="container-fluid">
        <!--row 1
          col-md-3 col-sm-3
          col-md-6 col-sm-6
          col-md-3 col-sm-3-->
        <div class="row">
          <div class="col-2 pt-4 pb-2">
            <!--logo image-->
            <div class="logo me-3">
              <img :src="imgLogo" alt="logo" height="60px" width="60px" />
            </div>
          </div>
          <!--end of logo-->

          <!--Title-->
          <div class="col-10 pt-4 pb-1">
            <h3>
              <b>Tiny Tasters</b>
              <small> E-Cake Shop</small>
              <img :src="imgGif" alt="" height="70px" width="70px" />
            </h3>
          </div>
          <!--end of title-->
        </div>
      </div>
    </div>
  </div>

  <!--End of row 1-->

  <body class="pic">
    <!--Search button final-->

    <div class="container pt-3 d-flex">
      <div class="row">
        <div class="col-8">
          <form class="d-flex" role="search">
            <input
              class="form-control me-2"
              type="search"
              placeholder="Search"
              aria-label="Search"
            />
            <button class="searchb btn btn-outline-dark rounded-pill" type="submit">Search</button>
          </form>
        </div>
        <div class="col-4">
          <RouterLink to="/booking-form"
            ><button class="searchb btn book-now-btn btn-outline-dark rounded-pill">
              Book Now
            </button></RouterLink
          >
        </div>
      </div>
    </div>
    <!--end of header-->

    <div class="container">
      <div class="row ms-2 pt-3">
        <div class="col-2">
          <RouterLink to="/browsing-2"
            ><img :src="imgButton" width="45px" height="40px"
          /></RouterLink>
        </div>
        <div class="container col-10">
          <h5 class="pt-2"><b>Games</b></h5>
        </div>
      </div>
    </div>

    <!--Row 1-->
    <div class="space container pb-5">
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/minecraft-1-details">
              <img :src="img1" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Minecraft 1</h4>
              <p class="card-text"><small class="text-white">₱ 1,000.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/minecraft-2-details">
              <img :src="img2" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Minecraft 2</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 1 end-->

      <!--row 2-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/roblox-details">
              <img :src="img3" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Roblox</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/biker-street-details">
              <img :src="img4" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Biker Street</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 2 end-->

      <!--row 3-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/moto-x3m-details">
              <img :src="img5" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">MOTO X3M</h4>

              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/mobile-legends-details">
              <img :src="img6" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Mobile Legends</h4>
              <p class="card-text"><small class="text-white">₱ 800.00 </small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 3 end-->
    </div>

    <br />

    <br />

    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <!-- Footer -->
    <br />
    <div class="bg-warning-subtle">
      <div class="container-fluid bottom-nav pt-2 pb-2">
        <div class="row text-center">
          <div class="col-3 text-white text-center">
            <RouterLink to="/#" title="Home">
              <i class="bi bi-house-door-fill"></i><br
            /></RouterLink>
            Home
          </div>
          <div class="col-3 text-white text-center">
            <RouterLink to="/#" title="Bookings"
              ><i class="bi bi-calendar2-range-fill"></i><br
            /></RouterLink>
            Your Bookings
          </div>
          <div class="col-3 text-white text-center">
            <RouterLink to="/#" title="Profile"
              ><i class="bi bi-person-circle"></i><br
            /></RouterLink>
            Profile
          </div>
          <div class="col-3 text-white text-center pe-4">
            <RouterLink to="/#" title="Profile"
              ><img :src="imgLogo" alt="" width="50px" class="footer-logo pt-1 pb-2" /><br
            /></RouterLink>
            About
          </div>
        </div>
      </div>
    </div>

    <!--End of footer-->
  </body>
</template>

<style scoped>
.btn-view {
  color: white;
  font-size: small;
  height: 30px;
  width: 75px;
  margin-left: 50px;
  background-color: orangered;
}
.header {
  background-color: #fe6803;
  background-color: #fe6803;
  text-shadow:
    -1px 0 white,
    0 1px white,
    1px 0 white,
    0 -1px white;
}
body .whitebody {
  background: white;
}

.bottom-nav {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: smaller;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background-color: #fe6803;
  z-index: 1000;
  box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.2);
}

.bi-house-door-fill {
  color: black;
  font-size: 30px;
}

.bi-calendar2-range-fill {
  color: black;
  font-size: 30px;
}

.bi-person-circle {
  color: black;
  font-size: 30px;
}
.fa-footer {
  background-color: #fe6803;
}

.img-cocomelon {
  height: 1000%;
}

body img {
  height: 100%;
}

.bi-search {
  font-size: 20px;
  background-color: #ffc96f;
}

.footer-logo {
  height: auto;
}

.searchb {
  background-color: #fe6803;
  color: white;
}
small {
  font-family:
    system-ui,
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    Oxygen,
    Ubuntu,
    Cantarell,
    'Open Sans',
    'Helvetica Neue',
    sans-serif;
}

.pic {
  height: auto;
  width: auto;
  background-color: #fee3d2;
}

.card {
  color: white;
  background-color: #000000;
}

.card p {
  color: white;
}

.card h4 {
  font-size: medium;
  font-family: 'Lucida Handwriting', cursive;
}
.space {
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
}
</style>
