<script>
import TheHeader from "./components/TheHeader.vue";
import TheFirstContent from "./components/TheFirstContent.vue";
import TheFooter from "./components/TheFooter.vue";
import TheBlueBanner from "./components/TheBlueBanner.vue";

export default {
  components: {
    TheHeader,
    TheFirstContent,
    TheFooter,
    TheBlueBanner
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
    <TheBlueBanner></TheBlueBanner>
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



}


</style>