<template>
  <div class="navbar-wrapper d-flex flex-column justify-center align-center pt-6">
    <div
      class="navbar-content d-flex flex-row justify-space-between align-center"
    >
      <div class="logo-wrapper d-flex align-center">
        <img src="@/assets/logo.svg" alt="" width="130px" />
      </div>
      <div
        class="option-wrapper d-flex flex-row justify-space-between align-center"
      >
        <div class="option">Fields</div>
        <div class="option">Services</div>
        <div class="option">Work</div>
        <div class="option">About</div>
        <!-- <v-btn class="start-button rounded-pill" variant="outlined"> Start a project 

          <img class="ml-1" src="@/assets/arrow-right.svg" alt="">
        </v-btn> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavbarComponent",
};
</script>

<style lang="scss">
.navbar-wrapper {
  top: 0px;
  left: 0px;
  // padding: 20px 250px;
  width: 100%;
  position: fixed;
  z-index: 10000000;

  .navbar-content {
    width: 80%;
    position: relative;
    z-index: 99999;
    background: rgba(0, 0, 0, 0.43);
    backdrop-filter: blur(6px);
    padding: 20px 50px;
    border-radius: 40px;
    .logo-wrapper {
      flex: 1;
    }
    .option-wrapper {
      flex: 1;

      .option {
        font-size: 17px;
      }
      .start-button {
        .v-btn__content {
          text-transform: capitalize !important;
          font-size: 17px;
        }
      }
    }
  }
}
</style>
