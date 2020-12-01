<template>
  <div id="app">
    <div id="nav">
      <Navbar />
    </div>
    <div class="header">
      <div class="row h-100 mb-2">
        <div class="col col-3 justify-content center h-100 p-1 logo">
          <b-avatar src="./assets/ship-logo.png" size="6rem"></b-avatar>
        </div>
        <div class="col col-9 h-100 p-1 pr-0 logo">
          <h5 class="heading " align="left">
            Cafe Canopic
            <h6 class="heading pl-2 pr-2" align="right">
              <b-badge pill variant="success" size="sm" width="10%"
                >OPEN</b-badge
              >
            </h6>
          </h5>
          <p class="pt-1">24 Long Neck Road, Wareham, MA, 02050</p>
          <div>
            <b-badge pill variant="light mr-3">Later</b-badge>
            <b-badge pill variant="light mr-3">Today</b-badge>
            <b-badge pill variant="light mr-3">10:30 AM</b-badge>
            <b-icon
              variant="primary"
              icon="pencil-square"
              font-scale="1"
            ></b-icon>
          </div>
        </div>
      </div>
    </div>
    <div class="menu p-3">
      <div class="row p-2 align-content-center">
        <div class="col-6 align-content-center ">
          <h5 class="menu-heading">Menu</h5>
        </div>
        <div class="col-6 align-content-right" align="right">
          <b-dropdown
            id="dropdown-1"
            text="Iced Drink"
            class="m-md-5 dropdown"
            align="right"
            variant="outline-dark"
            size="sm"
          >
            <b-dropdown-item>Iced Drink</b-dropdown-item>
            <b-dropdown-item>Coffee</b-dropdown-item>
            <b-dropdown-item>Tea</b-dropdown-item>
            <b-dropdown-divider variant="light"></b-dropdown-divider>
            <b-dropdown-item>Donots</b-dropdown-item>
            <b-dropdown-item>Cakes</b-dropdown-item>
            <b-dropdown-item>Biscuits</b-dropdown-item>
          </b-dropdown>
        </div>
      </div>
    </div>
    <div class="container">
      <h4 class="menu-item">Iced Drinks</h4>
      <div class="row sub-item mb-3 p-2">
        <div class="col-6" align="left">Iced Latte</div>
        <div class="col-6 price" align="right">$5.06</div>
      </div>
      <div class="row sub-item mb-3 p-2">
        <div class="col-6" align="left">Iced Mocha</div>
        <div class="col-6 price" align="right">$5.72</div>
      </div>
      <div class="row sub-item mb-3 p-2">
        <div class="col-6" align="left">Iced Brew</div>
        <div class="col-6 price" align="right">$5.28</div>
      </div>
      <div class="row sub-item mb-3 p-2">
        <div class="col-6" align="left">Iced Mocha Latte</div>
        <div class="col-6 price" align="right">$6.27</div>
      </div>
    </div>
    <div class="footer p-3">
      <button class="notification">2</button>
      <b-icon icon="cart4" style="color:white;" font-scale="2"> </b-icon>
      <h5 class="view-cart" style="float:right;">View Cart</h5>
    </div>
  </div>
</template>
<script>
import Navbar from "./components/Navbar";
export default {
  name: "App",
  components: {
    Navbar,
  },
};
</script>

<style>
#app {
  background-color: #f5f8f6;
}
.notification {
  background: #f6423e;
  border: 1px solid #f6423e;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  color: white;
  margin-right: 10px;
}
/* custom tag */
.custom-icons {
  display: inline;
}
h4 {
  display: inline;
}
h5 {
  display: inline;
}

h6 {
  display: inline;
}
p {
  font-family: "Lato", sans-serif;
  font-family: "Noto Sans", sans-serif;
  font-family: "Open Sans", sans-serif;
  font-family: "Poppins", sans-serif;
  color: rgb(173, 166, 166);
  font-size: 73%;
  font-weight: bold;
}
b-badge {
  background-color: darkgrey;
}
/* custom-classes */
/* .custom-jumbo{
  width: 100%;
  height: 100%;

} */
.header {
  background-color: #fff;
  padding: 8%;
}
.main-img {
  width: 100%;
  height: 60%;
  border: 1px solid grey;
  border-image: round;
}
.heading {
  font-family: "Lato", sans-serif;
  font-family: "Noto Sans", sans-serif;
}
.light {
  background-color: darkgray;
}
.menu {
  background-color: #f5f8f6;
}

.menu-heading {
  color: darkgrey;
  position: inline;
}
.dropdown {
  position: inline;
  padding-right: 0%;
  background-color: #fff;
}
.menu-item {
  color: rgb(87, 87, 84);
}

.sub-item {
  background-color: #fff;
  font-family: "Lato", sans-serif;
  font-family: "Noto Sans", sans-serif;
  font-family: "Open Sans", sans-serif;
  font-family: "Poppins", sans-serif;
  font-family: "Roboto", sans-serif;
  font-size: 15px;
  color: rgb(145, 139, 139);
}
.price {
  color: rgb(22, 165, 165);
  font-weight: bolder;
}

/* footer */
.footer {
  background-color: rgb(206, 126, 126);
}
.view-cart {
  color: #fff;
}

/* custom-id */
</style>
