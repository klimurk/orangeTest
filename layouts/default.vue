<template>
  <v-app >
    <div>
    <b-navbar toggleable="lg"  fixed class="nav bg-transparent">
      <b-navbar-brand href="#" class="nav_text"><img src="~assets/img/logo.svg" alt=""></b-navbar-brand>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto fs-5">
          <b-nav-item-dropdown text="Tools" right class="mr-11" >
            <b-dropdown-item href="#">Tool1</b-dropdown-item>
            <b-dropdown-item href="#">Tool2</b-dropdown-item>
            <b-dropdown-item href="#">Tool3</b-dropdown-item>
            <b-dropdown-item href="#">Tool4</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown text="Resources" right class="mr-11">
            <b-dropdown-item href="#">Resources1</b-dropdown-item>
            <b-dropdown-item href="#">Resources2</b-dropdown-item>
            <b-dropdown-item href="#">Resources3</b-dropdown-item>
            <b-dropdown-item href="#">Resources4</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item href="" class="mr-11 clr-black">Pricing</b-nav-item>
          <button class="btn btn-lg btn-sign mr-11 text-white">Sign Up</button>
          <b-nav-item href="" >Log In</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
    <v-main>
      <!-- <v-container> -->
        <Nuxt />
      <!-- </v-container> -->
    </v-main>

  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {

    }
  },
}
</script>

<style lang="scss" scoped>
// @font-face {
//   font-family: "HelveticaNowDisplay";
//   src: local("HelveticaNowDisplay"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Regular.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Black.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Bold.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-ExtLt.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Light.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Thin.ttf') format("truetype"),
//    url('~assets/fonts/HelveticaNowDisplay/HelveticaNowDisplay-Medium.ttf') format("truetype");
// }
// @import "node_modules/bootstrap/scss/functions";
// @import "node_modules/bootstrap/scss/variables";
// @import "node_modules/bootstrap/scss/mixins";
  .nav{
    padding: 45px 65px;
    font-family: "HelveticaNowDisplay";
    .btn-sign{
      background-color: $clr-rose;
      transition: $transition-base ;
      &:hover{
        background-color: $red-500;
      }
    }
    // .nav_text {
    //   color: $clr-black !important;
    // }

  }
  .navbar-light::v-deep .navbar-nav .nav-link{
    color:  $clr-black !important;
    >span{
      color:  $clr-black !important;
    }
  }
</style>
