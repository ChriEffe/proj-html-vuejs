<template>
  <main>
    <div class="container">
      <!-- shop info -->
      <div class="row shop-info fw-bold">
        <div class="col-3 d-flex justify-content-center align-items-center">
          <i class="far fa-clock"></i> 24/7 delivery
        </div>
        <div class="col-3 d-flex justify-content-center align-items-center">
          <i class="fas fa-hamburger"></i> Over 100 dishes
        </div>
        <div class="col-3 d-flex justify-content-center align-items-center">
          <i class="fas fa-mobile-alt"></i> in app ordering
        </div>
        <div class="col-3 d-flex justify-content-center align-items-center">
          <i class="fas fa-car"></i> fast delivery
        </div>
      </div>
    </div>
    <!-- popular dishes -->
    <Popular />
    <!-- banner offer -->
    <div class="banner offer"></div>
    <!-- categories -->
    <Categories />
    <!-- banner app -->
    <div class="banner app">
      <div class="container">
        <div class="content">
          <h4 class="fs-1">Download Our</h4>
          <h1 class="mb-5">
            <span>Ordering App</span>
          </h1>
          <a href="#"
            ><img
              class="me-4"
              src="../assets/img/app-store-badge-200x67.png"
              alt="app store"
          /></a>
          <a href="#"
            ><img
              src="../assets/img/play-store-badge-200x67.png"
              alt="play store"
          /></a>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import Categories from "./Categories.vue";
import Popular from "./Popular.vue";

export default {
  name: "Main",
  components: {
    Categories,
    Popular,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

h2 {
  color: $black;
}
.shop-info {
  height: 60px;
  background-color: $white;
  text-transform: uppercase;
  color: $grey;
  margin-top: -30px;
  div i {
    color: $black;
    padding-right: 1em;
  }
}
.banner {
  height: 430px;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 5em;
}
.offer {
  background-image: url(../assets/img/first-order-background-scaled.jpg);
}
.app {
  background-image: url(../assets/img/app-ordering-scaled.jpg);
}
.content {
  color: $white;
  padding-top: 5em;
  h1 {
    font-weight: 900;
    font-size: 4em;
    span {
      color: $yellow;
    }
  }
}
</style>
