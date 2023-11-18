<script>
export default {

  data() {
    return {
      headerList: [
        'Characters',
        'Comics',
        'Movies',
        'Tv',
        'Games',
        'Collectibles',
        'Video',
        'Fans',
        'News',
        'Shop'
      ]

    }
  }


};
</script>

<template>
  <header class="py-2">
    <div class="container">
      <nav class="navbar navbar-expand-lg">
        <!-- Logo -->
        <div>
          <img src="../assets/img/dc-logo.png" alt="DC">
        </div>
        <!-- Toggler -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- List -->
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav text-center ms-lg-auto">
            <li class="nav-item" v-for="singleElement in headerList">
              <a class="nav-link text-uppercase" href="#">{{ singleElement }}</a>
            </li>
          </ul>
        </div>

      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
  font-family: $font-primary;
  padding-bottom: 1rem;

  img {
    width: 70px;
  }

  .navbar-nav {
    font-size: .8rem;
    font-weight: 600;


    a {
      color: $color-text;

      &:hover {
        color: $color-primary;
        border-bottom: 1px solid $color-primary;
      }
    }
  }
}
</style>