<script>
import TheHeader from "./components/TheHeader.vue";
import TheFirstContent from "./components/TheFirstContent.vue";
import TheBlueBanner from "./components/TheBlueBanner.vue";
import dcList from "./db/dc-comics.json"
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFirstContent,
    TheFooter,
    TheBlueBanner
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
  <TheFirstContent></TheFirstContent>

  <main>
    <TheBlueBanner></TheBlueBanner>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;



</style>