<script setup>
import imgCover from '@/assets/images/cover.png'
import imgButton from '@/assets/images/backbutton.png'
import imgLine from '@/assets/images/cursive line.png'
</script>

<template>
  <div class="header py-4">
    <div class="container">
      <div class="row ms-2">
        <div class="col-2">
          <RouterLink to="/browsing-1">
            <img :src="imgButton" width="55px" height="60px"
          /></RouterLink>
        </div>
        <div class="col-1 pt-2 pe-3">
          <i class="bi bi-newspaper ps-3"></i>
        </div>
        <div class="container col-9">
          <h2 class="pt-2 ps-4"><b>Booking Form</b></h2>
        </div>
      </div>
    </div>
  </div>

  <div>
    <img :src="imgCover" alt="Back" width="100%" height="300px" />
  </div>
  <body class="container-fluid">
    <br />
    <div>
      <h1 class="pt-3">
        <center>Book your best choice!</center>
      </h1>
    </div>
    <div class="text-center"><img :src="imgLine" width="75%" height="20%" /></div>
    <br />
    <div class="container row g-3 mx-1">
      <span>Enter Your Name:</span>
      <div class="col-5">
        <input type="text" class="form-control" placeholder="First name" aria-label="First name" />
      </div>
      <div class="col-5">
        <input type="text" class="form-control" placeholder="Last name" aria-label="Last name" />
      </div>

      <div class="col-2">
        <input type="text" class="form-control" placeholder="M.I." aria-label="M.I" />
      </div>
    </div>

    <br />
    <!--PHONE NUMBER-->
    <div class="container row g-3 mx-1">
      <div class="col-5">
        <label for="exampleFormControlInput1" class="form-label">Phone Number</label>
        <input type="text" class="form-control" placeholder="+63" aria-label="Phone Number" />
      </div>
      <!--FACEBOOK LINK-->
      <div class="col-7">
        <label for="exampleFormControlInput1" class="form-label">Facebook link:</label>
        <input
          type="text"
          class="form-control"
          placeholder="https//www/facebook/com"
          aria-label="Facebook link"
        />
      </div>
    </div>

    <br />
    <!--ADDRESS-->
    <div class="container row g-3 mx-1">
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Address</label>
        <input
          type="text"
          class="form-control"
          placeholder="street/barangay"
          aria-label="street/barangay"
        />
      </div>
      <div class="col-4">
        <label for="exampleFormControlInput1" class="form-label">Province</label>
        <input type="text" class="form-control" placeholder="province" aria-label="province" />
      </div>

      <div class="col-2">
        <label for="exampleFormControlInput1" class="form-label">ZIP</label>
        <input type="text" class="form-control" placeholder="" aria-label="  ZIP" />
      </div>
    </div>
    <!--END OF ADDRESS-->

    <br />

    <!-- Category, Theme, Design
    <div class="container row g-3 mx-1">
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Select Category</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Personalized Cake Design</option>
          <option value="2">Regular Cake Design</option>
        </select>
      </div>
    </div>
    <div class="container row g-3 mx-1">
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Select Design</label>
      </div>
    </div>
    Category selection
          <select v-model="selectedCategory" @change="onCategoryChange">
            <option value="" disabled selected>Please select a category</option>
            <option value="disneyPrincess">Disney Princesses</option>
            <option value="superheroes">Superheroes</option>
          </select>

          Dynamically shown options based on category selection
          <select v-if="selectedCategory" v-model="selected">
            <option value="" disabled selected>Please select an option</option>
            <option v-for="option in dynamicOptions" :key="option.value" :value="option.value">
              {{ option.text }}
            </option>
          </select>

           Display selected value
          <div class="mt-3">
            Selected: <strong>{{ selected }}</strong>
          </div>
        </div>
      </div>
    </div>

    <br />

     Flavor, Size, Shape
    <div class="container row g-3 mx-1">
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Select Flavor</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Choco Moist</option>
          <option value="2">Red Velvet</option>
          <option value="3">Butter Cake</option>
        </select>
      </div>
      <div class="col-3">
        <label for="exampleFormControlInput1" class="form-label">Size</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">10 x 2</option>
          <option value="2">8 x 4</option>
          <option value="3">6 x 5</option>
        </select>
      </div>
      <div class="col-3">
        <label for="exampleFormControlInput1" class="form-label">Shape</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Circle</option>
          <option value="2">Heart</option>
          <option value="3">Tall Cakes</option>
          <option value="4">Number Cakes</option>
        </select>
      </div>
    </div>

    <br />
   Color, Toppers
    <div class="container row g-3 mx-1">
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Select Color</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Blue</option>
          <option value="2">Yellow</option>
          <option value="3">Black</option>
          <option value="4">Violet</option>
          <option value="5">Orange</option>
          <option value="6">Green</option>
          <option value="7">Brown</option>
          <option value="8">Pink</option>
          <option value="9">Red</option>
        </select>
      </div>
      <div class="col-6">
        <label for="exampleFormControlInput1" class="form-label">Select Topper</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Printed Topper</option>
          <option value="2">Written Dedication</option>
        </select>
      </div>
    </div>
    <br />

  -->
    <!--group-->
    <div id="app container row g-3 mx-1">
      <div class="form-group mx-3">
        <label for="category">Select Category:</label>
        <select v-model="selectedCategory" @change="updateOptions">
          <option value="">--Choose a category--</option>
          <option value="personalized">Personalized Cake</option>
          <option value="regular">Regular Cake</option>
        </select>
      </div>

      <div v-if="selectedCategory === 'personalized'">
        <div class="form-group mx-3">
          <label for="theme">Select Theme:</label>
          <select v-model="selectedTheme" @change="updateDesigns">
            <option value="">--Choose a theme--</option>
            <option value="disney">Disney Characters</option>
            <option value="heroes">Super Heroes</option>
            <option value="flowbut">Flowers and Butterflies</option>
            <option value="barbie">Barbie</option>
            <option value="games">Games</option>
            <option value="cartoons">Cartoons</option>
            <!-- Add more themes as needed -->
          </select>
        </div>

        <div v-if="selectedTheme">
          <div class="form-group mx-3">
            <label for="design">Select Design:</label>
            <select v-model="selectedDesign">
              <option value="">--Choose a design--</option>
              <option v-for="design in availableDesigns" :key="design" :value="design">
                {{ design }}
              </option>
            </select>
          </div>
        </div>
      </div>

      <!-- Common options for both Personalized and Regular Cakes -->
      <div class="form-group mx-3">
        <label for="flavor">Select Flavor:</label>
        <select v-model="selectedFlavor">
          <option value="">--Choose a flavor--</option>
          <option value="choho">Choco moist</option>
          <option value="red">Red Velvet</option>
          <option value="butter">Butter cake</option>
        </select>
      </div>

      <div class="form-group mx-3">
        <label for="size">Select Size:</label>
        <select v-model="selectedSize">
          <option value="">--Choose a size--</option>
          <option value="large">10 x 2</option>
          <option value="medium">8 x 4</option>
          <option value="small">6 x 5</option>
        </select>
      </div>

      <div class="form-group mx-3">
        <label for="shape">Select Shape:</label>
        <select v-model="selectedShape" v-if="selectedCategory === 'personalized'">
          <option value="">--Choose a shape--</option>
          <option value="circle">Circle</option>
          <option value="heart">Heart</option>
          <option value="tall">Tall cakes</option>
        </select>
      </div>

      <div class="form-group mx-3">
        <label for="color">Select Color:</label>
        <select v-model="selectedColor">
          <option value="">--Choose a color--</option>
          <option value="blue">Blue</option>
          <option value="yellow">Yellow</option>
          <option value="black">Black</option>
          <option value="violet">Violet</option>
          <option value="orange">Orange</option>
          <option value="green">Green</option>
          <option value="brown">Brown</option>
          <option value="pink">Pink</option>
          <option value="red">Red</option>
        </select>
      </div>

      <div class="container row g-3 mx-1">
        <div class="col-12">
          <label for="inputlg" class="form-label">Message:</label>
          <input
            type="text"
            class="form-control input-lg"
            placeholder="Write your dedication here"
            aria-label="Phone Number"
          />
        </div>
      </div>
    </div>

    <!--End of group-->
    <br />
    <div class="container row ps-4">
      <div class="col-7">
        <label for="date">Select Date:</label>
        <form action="/action_page.php">
          <input type="date" id="date" name="date" class="py-2 px-4 rounded-3 text-muted" />
        </form>
      </div>
      <div class="col-5">
        <label for="time">Select Time:</label>
        <input
          type="time"
          id="time"
          name="time"
          min="09:00"
          max="18:00"
          required
          class="py-2 px-4 rounded-3 text-muted"
        />
      </div>
    </div>
    <br />
    <div class="container row g-3 mx-1">
      <div>
        <label for="exampleFormControlInput1" class="form-label">Delivery Option</label>
        <select class="form-select" aria-label="Default select example">
          <option selected></option>
          <option value="1">Pick-up</option>
          <option value="2">Door-to-Door</option>
        </select>
      </div>
    </div>

    <br /><br />
    <div class="container d-grid">
      <div class="text-center">
        <button class="btn btn-danger" type="button">Submit</button>
      </div>
    </div>

    <br /><br />
  </body>
</template>

<style scoped>
@import url('https://fonts.cdnfonts.com/css/mistrully');

.header {
  background: linear-gradient(to left, orange 0%, orangered 100%);
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial,
    sans-serif;
}
.header h2 {
  font-family: 'Dancing Script', cursive;
}
body {
  background: lightgray;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

body h1 {
  font-family: 'Mistrully', sans-serif;
  font-size: 45px;
}

.form-group {
  margin-bottom: 1em;
}

select {
  width: 100%;
  padding: 0.5em;
  font-size: 1em;
  margin-top: 0.3em;
}

i {
  font-size: 25px;
}
</style>

<script>
export default {
  data() {
    return {
      selectedCategory: '',
      selectedTheme: '',
      selectedDesign: '',
      selectedFlavor: '',
      selectedSize: '',
      selectedShape: '',
      selectedColor: '',
      selectedToppers: '',
      availableDesigns: [],
    }
  },
  methods: {
    updateOptions() {
      if (this.selectedCategory === 'personalized') {
        // Show the theme and design options for personalized cakes
        this.updateDesigns() // Automatically update designs based on theme selection
      } else {
        // Reset the theme and design options when "Regular Cake" is selected
        this.selectedTheme = ''
        this.selectedDesign = ''
        this.availableDesigns = []
      }
    },
    updateDesigns() {
      // Update design options based on the selected theme
      if (this.selectedTheme === 'disney') {
        this.availableDesigns = [
          'Elsa',
          'Ariel',
          'Rapunzel',
          'Anna',
          'Cinderella',
          'Sofia',
          'Snow White',
          'Mickey Mouse',
          'Minion',
          'Miraculous',
          'Cars',
          'Tinkerbell',
        ]
      } else if (this.selectedTheme === 'heroes') {
        this.availableDesigns = [
          'Spider-Man 1',
          'Spider-Man 2',
          'Spider-Man 3',
          'Spider-Man 4',
          'Spider-Man 5',
          'Hulk 1',
          'Hulk 2',
          'Batman 1',
          'Batman 2',
          'Captain America',
        ]
      } else if (this.selectedTheme === 'flowbut') {
        this.availableDesigns = [
          ' Design 1',
          ' Design 2',
          ' Design 3',
          ' Design 4',
          ' Design 5',
          ' Design 6',
          ' Design 7',
          'Desgin 8',
          'Design 9',
          'Design 10',
        ]
      } else if (this.selectedTheme === 'games') {
        this.availableDesigns = [
          'Mobile Legend',
          'Minecraft',
          'Roblox',
          'Biker Street',
          'Moto X3M Pool Party',
        ]
      } else if (this.selectedTheme === 'barbie') {
        this.availableDesigns = [
          'Barbie 1',
          'Barbie 2',
          'Barbie 3',
          'Barbie 4',
          'Barbie 5',
          'Barbie 6',
        ]
      } else if (this.selectedTheme === 'cartoons') {
        this.availableDesigns = [
          'Cocomelon',
          'Paw Patrol',
          'Hello Kitty',
          'Spongebob',
          'Peppa Pig',
          'Kuromi',
          'Unicorn',
          'Little Charmers',
        ]
      } else {
        this.availableDesigns = []
      }
    },
  },
}
</script>
