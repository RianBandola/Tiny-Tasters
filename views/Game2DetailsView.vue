<script setup>
import img2 from '@/assets/images/Minecraft 2.png'
import imgLogo from '@/assets/images/tiny taster logo.png'
import imgGif from '@/assets/images/gif 2.gif'
import imgButton from '@/assets/images/backbutton.png'
</script>

<template>
  <div class="bg-warning">
    <div class="header">
      <div class="container-fluid">
        <!--row 1-->
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
  <!-- End row 1-->
  <div>
    <div class="card">
      <img :src="img2" class="card-img-top object-fit-cover rounded-0" alt="" />
      <div class="card-img-overlay">
        <RouterLink to="/browsing-7"
          ><img :src="imgButton" width="45px" height="40px"
        /></RouterLink>
      </div>
    </div>
  </div>
  <body class="pic pb-5 bg-white">
    <!--Search button final-->

    <div class="container pt-3 d-grid">
      <div class="row">
        <!--ratings-->
        <div class="col-4">
          <h1 class="mt-2">₱ 800.00</h1>
        </div>
        <div class="col">
          <div class="rating pb-1">
            <span
              v-for="star in stars"
              :key="star"
              :class="['star', { active: star <= currentRating, disabled }]"
              @click="!disabled && updateRating(star)"
            >
              ★
            </span>
          </div>
        </div>

        <!--Ratings end-->

        <div class="col mt-2">
          <RouterLink to="/booking-form">
            <button class="searchb btn book-now-btn btn-md btn-outline-dark rounded-pill">
              Book
            </button></RouterLink
          >
        </div>
      </div>
    </div>

    <div class="rounded-box rounded-3 mx-3">
      <h1><b>Minecraft 2</b></h1>

      <p>
        This is a beautiful Minecaft themed cake, perfect for a birthday party or any special
        occasion. It features a figurine of Minecaft, a blue frosted cake decorated with white
        snowflakes. This cake is sure to be a hit with any Frozen fan!
      </p>
    </div>

    <div class="container px-3">
      <div class="card-group d-flex pt-3 row justify-content-center">
        <div class="card col-md-3 bg-transparent">
          <div class="card-body ms-0">
            <h5 class="card-title">Flavor</h5>
            <small class="card-text">
              <li>Choco Moist</li>
              <li>Red Velvet</li>
              <li>Butter Cake</li>
            </small>
            <hr />
            <h5 class="card-title">Toppers</h5>
            <small class="Toppers">
              <li>Printed</li>
              <li>Dedication</li>
              <li>Candle</li>
            </small>
          </div>
        </div>
        <div class="card">
          <div class="card-body col-md-3 ms-0 bg-transparent">
            <h5 class="card-title">Size</h5>
            <small class="card-text">
              <li>10 x 2</li>
              <li>8 x 4</li>
              <li>6 x 5</li>
            </small>
            <hr />

            <h5 class="card-title">Shape</h5>
            <small class="card-text">
              <li>Circle</li>
              <li>Heart</li>
              <li>Tall Cakes</li>
            </small>
          </div>
        </div>
        <div class="card col-md-5">
          <div class="card-body bg-transparent">
            <h5 class="card-title">Color</h5>
            <small class="card-text mx-1">
              <li>Blue</li>
              <li>Black</li>
              <li>Yellow</li>
              <li>Violet</li>
              <li>Orange</li>
              <li>Green</li>
              <li>Brown</li>
              <li>Pink</li>
            </small>
          </div>
        </div>
      </div>
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
.header {
  background-color: #fe6803;
  text-shadow:
    -1px 0 white,
    0 1px white,
    1px 0 white,
    0 -1px white;
}
.searchb {
  background-color: #fe6803;
  color: white;
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

.pic img {
  height: 100%;
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
  width: fit-content;
}

.space {
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
}

body {
  background-color: #eee;
}

.rating {
  display: flex;
  font-size: 30px;
}
.star {
  cursor: pointer;
  padding: 5px;
  color: #ccc;
}
.star.active {
  color: #f39c12;
}
.star.disabled {
  cursor: not-allowed;
}
.rounded-box {
  padding: 15px 15px;
  font-family: 'Lucida Handwriting', cursive;
  font-size: 24px;
  font-weight: bold;
  color: black;
  background-color: #fadadd;
  text-align: left;
  display: inline-block;
}

.rounded-box p {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  font-size: medium;
}

hr {
  border: solid;
  border-color: black;
}
.card {
  background: linear-gradient(to left, orange 0%, orangered 100%);
  color: black;
}
</style>

<script>
export default {
  props: {
    value: {
      type: Number,
      default: 0,
    },
    max: {
      type: Number,
      default: 5,
    },
    disabled: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
      currentRating: this.value,
    }
  },
  computed: {
    stars() {
      return Array.from({ length: this.max }, (_, i) => i + 1)
    },
  },
  methods: {
    updateRating(star) {
      this.currentRating = star
      this.$emit('input', star)
    },
  },
}
</script>
