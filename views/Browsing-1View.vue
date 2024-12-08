<script setup>
import img1 from '@/assets/images/personalized cake design.jpg'
import img2 from '@/assets/images/regular cake 3.png'
import imgLogo from '@/assets/images/tiny taster logo.png'
import imgGif from '@/assets/images/gif 2.gif'
</script>

<template>
  <body class="bg-warning-subtle">
    <div>
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

    <!--Search button final-->

    <div class="container pt-3">
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

    <!-- Personalized Cake Design -->
    <div class="container my-4 pt-5">
      <div class="card mb-3 custom-card ps-2 py-2 rounded-5">
        <div class="row g-0 align-items-center">
          <!-- Image Section -->
          <div class="col-4">
            <img :src="img1" alt="Cake Image" class="img-fluid card-img rounded-5" />
          </div>

          <!-- Content Section -->
          <div class="col-8">
            <div class="card-body">
              <h5 class="custom-card-title">Personalized Cake Design</h5>
              <div class="text-end">
                <RouterLink to="/browsing-2">
                  <button class="btn btn-view text-center rounded-1 mt-3 mb-2 ms-5 m-4">
                    View
                  </button>
                </RouterLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End of Personalized Cake Design -->
    <!-- Regular Cake Design -->
    <div class="container my-4 pb-5">
      <div class="card mb-3 custom-card ps-2 py-2 rounded-5">
        <div class="row g-0 align-items-center">
          <!-- Image Section -->
          <div class="col-4">
            <img :src="img2" alt="Cake Image" class="img-fluid card-img rounded-5 p-1" />
          </div>

          <!-- Content Section -->
          <div class="col-8">
            <div class="card-body">
              <h5 class="custom-card-title">Regular Cake Design</h5>
              <div class="text-center">
                <RouterLink to="/regular-browsing">
                  <button class="btn btn-view float-end rounded-1 mt-3 mb-2 ms-5 m-4">View</button>
                </RouterLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <!-- End of Regular Cake Design -->

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
</style>
