<script setup>
import img1 from '@/assets/images/regular 1.png'
import img2 from '@/assets/images/regular 2.png'
import img3 from '@/assets/images/regular 3.png'
import img4 from '@/assets/images/regular 4.png'
import img5 from '@/assets/images/regular 5.png'
import img6 from '@/assets/images/regular 6.png'
import img7 from '@/assets/images/regular 7.png'
import img8 from '@/assets/images/regular 8.png'
import img9 from '@/assets/images/regular 9.png'
import img10 from '@/assets/images/regular 10.png'
import img11 from '@/assets/images/regular 11.png'
import img12 from '@/assets/images/regular 12.png'
import img13 from '@/assets/images/regular 13.png'
import img14 from '@/assets/images/regular 14.png'

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
          <RouterLink to="/browsing-1"
            ><img :src="imgButton" width="45px" height="40px"
          /></RouterLink>
        </div>
        <div class="container col-10">
          <h5 class="pt-2"><b>Regular Cake Design</b></h5>
        </div>
      </div>
    </div>

    <!--Row 1-->
    <div class="space container pb-5">
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-1-details">
              <img :src="img1" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 1</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-2-details">
              <img :src="img2" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 2</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 1 end-->

      <!--row 2-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-3-details">
              <img :src="img3" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 3</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-4-details">
              <img :src="img4" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 4</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 2 end-->

      <!--row 3-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-5-details">
              <img :src="img5" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 5</h4>

              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-6-details">
              <img :src="img6" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 6</h4>
              <p class="card-text"><small class="text-white">₱ 650.00 </small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 3 end-->

      <!--row 4-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-7-details">
              <img :src="img7" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 7</h4>
              <p class="card-text"><small class="text-white">₱ 400.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-8-details">
              <img :src="img8" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 8</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 4 end-->

      <!--row 5-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-9-details">
              <img :src="img9" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 9</h4>
              <p class="card-text"><small class="text-white">₱ 650.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-10-details">
              <img :src="img10" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 10</h4>
              <p class="card-text"><small class="text-white">₱ 400.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 5 end-->

      <!--row 5-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-11-details">
              <img :src="img11" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 11</h4>
              <p class="card-text"><small class="text-white">₱ 650.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-12-details">
              <img :src="img12" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 12</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 5 end-->

      <!--row 6-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-13-details">
              <img :src="img13" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 13</h4>
              <p class="card-text"><small class="text-white">₱ 650.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/regular-cake-14-details">
              <img :src="img14" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Regular 14</h4>
              <p class="card-text"><small class="text-white">₱ 650.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 6 end-->
    </div>

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
  font-family: 'Lucida Handwriting', cursive;
}
.space {
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
}
</style>
