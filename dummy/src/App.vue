<template>
  <div id="app">
    <div id="nav">
      <Nav />
    </div>

    <div class="container pr-3 pl-3 pt-0">
      <h5 class="location">Store Location</h5>
      <!-- Bay village -->
      <div class="row radio row-12 p-2 m-1 mb-3">
        <div class="custom-control custom-radio">
          <input type="radio" name="customRadio" class="custom-control-input" />
          <label
            class="custom-control-label universal location-sub"
            for="customRadio1"
            >Bay Village</label
          >
        </div>
      </div>
      <!-- Charles Town -->
      <div class="row radio row-12 p-2 m-1 mb-3">
        <div class="custom-control custom-radio">
          <input type="radio" name="customRadio" class="custom-control-input" />
          <label
            class="custom-control-label universal location-sub"
            for="customRadio1"
            >Charles Town</label
          >
          <p class="m-0 address">
            2244, Belly drive, Charles estown, Boston, MA, 2541A
          </p>
          <p class="m-0 address">844 mtrs</p>
        </div>
      </div>
    </div>

    <div class="container p-1">
      <div class=" row-12  ">
        <div class="col-12" align="center">
          <div class="btn-group " role="group">
            <button class="universal button  ">ASAP</button>
            <button class="universal button ">Later</button>
          </div>
        </div>
      </div>
    </div>

    <div class="container p-3 pt-0">
      <div id="scroll-bar" class="row-12 mb-2">
        <div class="col-12" align="center">
          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Today</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:00 AM</p>
            </div>
          </div>

          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Tomorrow</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:15 AM</p>
            </div>
          </div>
          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Sep 24 Fri</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:20 AM</p>
            </div>
          </div>

          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Sep 25 Sat</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:25 AM</p>
            </div>
          </div>

          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Sep 26 Sun</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:30 AM</p>
            </div>
          </div>

          <div class="row-12 m-2">
            <div class="col-6 scedule" align="center">
              <button class="universal  day-button">Sep 27 Mon</button>
            </div>
            <div class="col-6 scedule" align="center">
              <p>10:35 AM</p>
            </div>
          </div>
        </div>
      </div>

      <div class="row-12">
        <div class="col-12" align="center">
          <button class="universal update ">Update</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Nav from "./components/Nav";
export default {
  name: "App",

  components: {
    Nav,
  },
};
</script>
<style lang="scss">
// ID SELECTOR
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#scroll-bar {
  height: 200px;
  width: 100%;
  overflow-y: auto;
}

::-webkit-scrollbar {
  width: 8px;

  background: rgb(212, 210, 210);
  border-radius: 20px;
}

::-webkit-scrollbar-thumb {
  background: #3797a4;
  border-radius: 20px;
  min-height: 5px;
}

// CLASS SELECTOR

// UNIVERSAL
.universal {
  color: #3797a4;
}

.row.radio {
  -moz-box-shadow: 0 0 3px #ccc;
  -webkit-box-shadow: 0 0 3px #ccc;
  box-shadow: 0 0 5px rgb(167, 164, 164);
}

.row.radio:hover {
  background-color: #e8fdff;
}

.location {
  font-weight: bold;
  color: rgb(43, 42, 42);
}

.location-sub {
  font-weight: bold;
}

// RADIO BUTTON

.custom-control-label::before {
  // background-color: darkorange;  /* orange */
}

/* This is the checked state */
.custom-control-input:checked ~ .custom-control-label::before,
.custom-control-input:checked ~ .custom-control-label::after {
  background-color: #3797a4;
  /* green */
  /* this bg image SVG is just a white circle, you can replace it with any valid SVG code */
  border-radius: 50%;
}

.address {
  color: rgb(134, 130, 130);
  font-size: 15px;
}

// button
.btn-custom {
  border: 1px solid #3797a4;
}

.btn-custom button {
  border: 1px solid #3797a4;
}

.scedule {
  display: inline-block;
}

.scedule-left {
  text-align: left;
}

.scedule-right {
  text-align: right;
}

.button {
  color: #3797a4;
  background: white;
  border: 1px solid rgb(212, 207, 207);
  padding-left: 5px;
  padding-right: 5px;
  width: 100%;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 5px;
  padding-bottom: 5px;
  box-shadow: 0 0 2px rgb(167, 164, 164);
}

.button:hover {
  background-color: #e8fdff;
  border: 1px solid rgb(212, 207, 207);
}

.day-button {
  color: #3797a4;
  background: white;
  border: 1px solid rgb(212, 207, 207);

  width: 100%;
  padding-left: 5px;
  padding-right: 5px;
  padding-top: 5px;
  padding-bottom: 5px;
  box-shadow: 0 0 2px rgb(167, 164, 164);
}

.day-button:hover {
  background-color: #e8fdff;
  border: 1px solid rgb(212, 207, 207);
}

.update {
  color: #3797a4;
  background: white;
  border: 1px solid rgb(212, 207, 207);
  padding-left: 25px;
  padding-right: 25px;
  padding-top: 8px;
  padding-bottom: 8px;
  font-weight: bolder;
  border-radius: 5px;
  box-shadow: 0 0 2px rgb(167, 164, 164);
}

.update:hover {
  background-color: #e8fdff;
  border: 1px solid rgb(212, 207, 207);
}

.day-button:visited {
  color: #fff;
  background: #3797a4;
  border: 1px solid #3797a4;
}
</style>
