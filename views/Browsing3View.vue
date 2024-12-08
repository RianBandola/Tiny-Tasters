<script setup>
import img1 from '@/assets/images/elsa.png'
import img2 from '@/assets/images/ariel.png'
import img3 from '@/assets/images/rapunzel.png'
import img4 from '@/assets/images/sofia.png'
import img5 from '@/assets/images/anna.png'
import img6 from '@/assets/images/cinderella.png'
import img7 from '@/assets/images/miraculous.png'
import img8 from '@/assets/images/minion.png'
import img9 from '@/assets/images/snow white.png'
import img10 from '@/assets/images/mickey mouse.png'
import img11 from '@/assets/images/tinkerbell.png'
import img12 from '@/assets/images/cars.png'

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

    <div class="container px-3">
      <div class="row ms-2 pt-3">
        <div class="col-2">
          <RouterLink to="/browsing-2"
            ><img :src="imgButton" width="45px" height="40px"
          /></RouterLink>
        </div>
        <div class="container col-10">
          <h5 class="pt-2"><b>Disney Characters</b></h5>
        </div>
      </div>
    </div>

    <!--Row 1-->
    <div class="space container pb-5">
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/elsa-details">
              <img :src="img1" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Elsa</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/ariel-details">
              <img :src="img2" class="card-img-top" alt="..." />
            </RouterLink>
            <div class="card-body">
              <h4 class="card-title">Ariel</h4>
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
            <RouterLink to="/rapunzel-details">
              <img :src="img3" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Rapunzel</h4>
              <p class="card-text"><small class="text-white">₱ 1,600.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/sofia-details">
              <img :src="img4" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Sofia</h4>
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
            <RouterLink to="/anna-details">
              <img :src="img5" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h5 class="card-title">Anna</h5>

              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/cinderella-details">
              <img :src="img6" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h5 class="card-title">Cinderella</h5>

              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 3 end-->

      <!--row 4-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/miraculous-details">
              <img :src="img7" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Miraculous</h4>
              <p class="card-text"><small class="text-white">₱ 800.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/minion-details"
              ><img :src="img8" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Minion</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 4 end-->
      <!--row 5-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/snow-white-details">
              <img :src="img9" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Snow White</h4>
              <p class="card-text"><small class="text-white">₱ 1,600.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/mickey-mouse-details">
              <img :src="img10" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h6 class="card-title">Mickey Mouse</h6>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 5 end-->

      <!--row 5-->
      <div class="row">
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/tinkerbell-details">
              <img :src="img11" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Tinker Bell</h4>
              <p class="card-text"><small class="text-white">₱ 800.00 </small></p>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="card mb-3">
            <RouterLink to="/cars-details"
              ><img :src="img12" class="card-img-top" alt="..."
            /></RouterLink>
            <div class="card-body">
              <h4 class="card-title">Cars</h4>
              <p class="card-text"><small class="text-white">₱ 800.00</small></p>
            </div>
          </div>
        </div>
      </div>
      <!--row 5 end-->
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
.card h5 {
  font-family: 'Lucida Handwriting', cursive;
}

.card h6 {
  font-family: 'Lucida Handwriting', cursive;
}
.space {
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
}
</style>
