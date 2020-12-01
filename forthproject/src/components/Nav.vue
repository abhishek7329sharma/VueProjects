<template>
  <b-container>
    <b-row class="p-2">
      <b-col align="left" class="">
        <p class="yourcart mt-2">Your cart</p>
      </b-col>
      <b-col align="right" class=" ">
        <p class="p mt-2 " style="font-weight:bold; color: #3797a4;">
          <b-icon icon="x" font-scale="1.5" style=""></b-icon>Close
        </p>
      </b-col>
    </b-row>
  </b-container>
</template>
<script>
export default {
  name: "Nav",
};
</script>

<style>
/* navbar styling */
/* ELEMENTS SELECTOR */
.yourcart {
  font-weight: bold;
  font-size: larger;
}
</style>
