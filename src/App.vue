<script>
import TheHeader from "./components/TheHeader.vue";
import TheFirstContent from "./components/TheFirstContent.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFirstContent,
    TheFooter,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <TheHeader></TheHeader>
  <TheFirstContent></TheFirstContent>

  <main>
    <div class="container">
      <div>
        <div>
          <img src="./assets/img/buy-comics-digital-comics.png" alt="digital-comics">
          <span>digital comics</span>
        </div>
        <div>
          <img src="./assets/img/buy-comics-merchandise.png" alt="dc-merchandise">
          <span>dc merchandise</span>

        </div>
        <div>
          <img src="./assets/img/buy-comics-subscriptions.png" alt="subscription">
          <span>subscription</span>

        </div>
        <div>
          <img src="./assets/img/buy-comics-shop-locator.png" alt="comic-shop">
          <span>comic shop locator</span>

        </div>
        <div>
          <img src="./assets/img/buy-dc-power-visa.svg" alt="dc-power" style="height: 50px;">
          <span>dc power visa</span>

        </div>
      </div>

    </div>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;


main {
  font-family: $font-primary;
  background-color: $color-primary;
  padding-top: 3rem;
  padding-bottom: 3rem;
  
  div{
    display: flex;
    justify-content: center;
    align-items: center;

    img{
      height: 60px;
      margin-left: 3rem;
      
    }

    
    span{
      font-size: .8rem;
      display: flex;
      padding-left: 1rem;
      text-transform:uppercase;
      color: white;
    }
  }
}

@for $i from 1 through 10 {
  .my-mt-#{$i} {
    margin-top: #{$i}rem;
  }
}

</style>