<template>
  <div>
    <section class="section1 d-flex flex-row">
      <!-- <div class="container"> -->
        <div class="section1__img position-relative col-8 ml-auto" >
          <b-img  src="~assets/img/block1back.png" class="w-100" />
          <h1 class="text-white position-absolute top-0 start-50  mt-20">Get sales, leads, and product reviews that you control!</h1>
          </div>
        <div class="section1__amazon position-absolute start-0 translate ">
          <h1 class="text-white mb-5  fw-bold word-break col-xxl-6">Amazon funnels</h1>
          <div class="d-flex flex-row justify-content-between align-items-center mb-5">
            <b-img src="~assets/img/stars.svg" />
            <h5 class="text-white mb-0">Based on reviews on</h5>
            <h5 class="text-white mb-0">
              <b-img src="~assets/img/carpeta.svg" />
              Capterra
            </h5>
          </div>
          <a class="btn section1__btn-blue btn-primary btn-lg text-white " href="#" role="button">Get started for free!</a>
        </div>
        <div class="section1__phone p-4 position-absolute bottom-0 end-0 d-flex flex-column">
          <div class="text-white mb-2 d-flex flex-row align-items-center">
            <b-img src="~assets/img/fate.svg" class="mr-2" />
            Fate
          </div>
          <h2 class="clr-green fs-4 mb-2">Fate® BioLite, <br/>  Anti-Aging Formula</h2>
          <b-img src="~assets/img/phone_inner.png" class="mb-2"/>
          <b-img src="~assets/img/dots.svg" height=10 />
          <div class="d-flex flex-row">
            <div class="col-6 pr-0 pl-0 d-flex flex-row align-items-center flex-wrap">
              <div class="phone__crossed ff-openSans clr-grey-light fs-6 mr-0">$47.42</div>
              <div class=" ff-openSans  border border-2 rounded-pill clr-yellow pr-2 pl-2 phone__sell ml-2">-55%</div>
              <div class="phone__price  ff-openSans d-flex">
                <div class="text-white   fs-3">$25</div>
                <div class="text-white   fs-6  d-inline">85</div>
              </div >
            </div>
            <div class="col-6  clr-grey-light text-uppercase phone__powered ff-openSans">
              powered by <br/>
              <b-img src="~assets/img/reward.svg"/>
              Elite rewards
            </div>
          </div>
          <a class="btn text-white bg-clr-rose btn-lg ff-openSans fs-6 mb-2" width href="#" role="button">Claim this rebate deal</a>

        <div class="phone__footer text-uppercase d-flex flex-row clr-grey-light ff-openSans align-items-center">
          <div class="clr-grey-light border border-2 rounded-circle text-lowercase pl-2 pr-2 mr-5"> i</div>
          Available at amazon
        </div>
          <!-- <b-img src="~assets/img/phone.png" class=/> -->
        </div>
        <b-img src="~assets/img/Laptop.png" class="section1__laptop position-absolute bottom-0 end-0 "/>
      <!-- </div> -->
    </section>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  layout:'default'
}
</script>

<style lang="scss" scoped>
// @font-face {
//   font-family: "Ovo";
//   src: local("Ovo"),
//    url('~assets/fonts/Ovo/Ovo-Regular.ttf') format("truetype");
// }
// @import "node_modules/bootstrap/scss/functions";
// @import "node_modules/bootstrap/scss/variables";
// @import "node_modules/bootstrap/scss/mixins";
  .section1{
    position: relative;
    &__img{
      margin-left: auto;
      transform: translateX(-45px);
      z-index: 1;
      &>h1{
        font-size: 48px;
        width: 435px;
        transform: translate(-90px,90px);
      }
    }
    &__amazon{
      background-color: $clr-rose;
      width: 630px;
      // height: 430px;
      z-index: 2;
      padding: 50px 70px;
      transform: translate(65px,70px);
      &>h1{
        font-size: 80px;
      }
    }
    &__btn-blue{
      background-color: $clr-blue;
      border-color: $clr-blue;
      transition:color .2s linear, border-color .2s linear;
      &:hover{
        background-color: $blue;
      border-color: $blue;
      }
    }
    &__laptop{
      z-index: 5;
      transform: translateY(130px) ;
    }
    &__phone{
      z-index: 6;
      transform: translate(-485px,70%);
      background-image: url(~assets/img/phone.png);
      background-size: contain;
      font-family: 'Ovo';
      max-width: 295/1440*100vw;
    }
  }
  .phone{
    &__crossed{
      position: relative;
      font-size: 14px;
      // font-family: Open Sans,sans-serif;
      // color: $clr-grey-light;
      &:before {
        content: "";
        border-bottom: 3px solid $clr-grey-light;
        position: absolute;
        width: 100%;
        height: 50%;
        transform: rotate(-12deg);
      }
    }
    &__sell{
      // font-family: Open Sans,sans-serif;
      border-color: $clr-yellow !important;
      font-size: 13px;
    }
    &__price{
      // font-family: Open Sans,sans-serif;
    }
    &__powered{
      font-size: 14px;
    }
  }
</style>