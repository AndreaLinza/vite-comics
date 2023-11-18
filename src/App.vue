<script>
import TheHeader from "./components/TheHeader.vue";
import TheFirstContent from "./components/TheFirstContent.vue";
import TheCardContent from "./components/TheCardContent.vue";
import dcList from "./db/dc-comics.json"
import TheBlueBanner from "./components/TheBlueBanner.vue";

import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFirstContent,
    TheBlueBanner,
    TheCardContent,
    TheFooter,
  },

  data() {
    return {
      dcList,
    };
  },



};
</script>

<template>
  <TheHeader></TheHeader>
  <main>
    <TheFirstContent></TheFirstContent>

    <section>
      <div class="container py-5">
        <div class=" row row-cols-2 row-cols-md-3 row-cols-lg-6 g-3">
          <div v-for="dcComics in dcList" class="col">

            <TheCardContent :thumb="dcComics.thumb" :series="dcComics.series"></TheCardContent>

          </div>
        </div>

      </div>
    </section>


    <TheBlueBanner></TheBlueBanner>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss" scoped>
@use "./styles/partials/variables" as *;

section {
    background-color: #303030;
    min-height: 400px;}
</style>