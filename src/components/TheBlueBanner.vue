<script>
export default {

  data() {
    return {
      // bannerList: [
      //     {

      //         imgBanner: [
      //             'buy-comics-digital-comics.',
      //             'buy-comics-merchandise.',
      //             'buy-comics-subscriptions.',
      //             'buy-comics-shop-locator.',
      //             'buy-dc-power-visa.',
      //         ],
      //         titleBanner: [

      //             'digital comics',
      //             'dc merchandise',
      //             'subscription',
      //             'comic shop locator',
      //             'dc power visa',
      //         ]


      //     }
      // ]

    }
  }

};
</script>

<template>
  <section class="blue-banner">
    <div class="container">
      <div class="row row-cols-1 row-cols-md-3 row-cols-lg-5 g-4 justify-content-center">

        <div class="col">
          <div class="d-flex justify-content-center">
            <a class="d-flex align-items-center" href="#">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              <span>digital comics</span>
            </a>
          </div>
        </div>

        <div class="col">
          <div class="d-flex justify-content-center">
            <a class="d-flex align-items-center" href="#">
              <img src="../assets/img/buy-comics-merchandise.png" alt="dc-merchandise">
              <span>dc merchandise</span>
            </a>
          </div>
        </div>

        <div class="col">
          <div class="d-flex justify-content-center">
            <a class="d-flex align-items-center" href="#">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
              <span>subscription</span>
            </a>
          </div>
        </div>

        <div class="col">
          <div class="d-flex justify-content-center">
            <a class="d-flex align-items-center" href="#">
              <img src="../assets/img/buy-comics-shop-locator.png" alt="comic-shop">
              <span>comic shop locator</span>
            </a>
          </div>
        </div>

        <div class="col">
          <div class="d-flex justify-content-center">
            <a class="d-flex align-items-center" href="#">
              <img src="../assets/img/buy-dc-power-visa.svg" alt="dc-power" style="height: 50px;">
              <span>dc power visa</span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

.blue-banner {
  font-family: $font-primary;
  background-color: $color-primary;
  padding-top: 2rem;
  padding-bottom: 2rem;
  min-height: 100px;



  img {
    height: 60px;
    margin-left: 3rem;

  }


  span {
    font-size: .8rem;
    display: flex;
    padding-left: 1rem;
    text-transform: uppercase;
    color: white;
  }
}
</style>