<template>
  <b-container>
    <b-row class="p-2">
      <b-col cols="12" align="right" class="p-2 text-align-center ">
        <p class="h5 mb-2 close" style=" ">
          <b-icon icon="x" font-scale="1.3" style=""></b-icon>Close
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
@import url("https://fonts.googleapis.com/css2?family=Poppins&family=Roboto:wght@100;400&display=swap");
/* navbar styling */
/* ELEMENTS SELECTOR */
.close {
  font-weight: bold !important;
  color: #057381 !important;
  font-family: "Poppins", sans-serif !important;
  font-family: "Roboto", sans-serif !important;
  font-size: 16px !important;
}
</style>
