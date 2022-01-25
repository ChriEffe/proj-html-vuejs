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
    <div class="popular container text-center">
      <h2 class="fw-bold">Our Most Popular Dishes</h2>
      <div class="row mb-4">
        <div class="col-4">
          <img src="../assets/img/skin-on-fries-400x571.jpg" alt="" />
          <h3>Skin On Fries</h3>
          <p>$3.00-$6.00</p>
        </div>
        <div class="col-4">
          <img src="../assets/img/choco-cookie-frappe-400x571.jpg" alt="" />
          <h3>Choko Cookie Frappe</h3>
          <p>$4.99</p>
        </div>
        <div class="col-4">
          <img src="../assets/img/donut-burger-400x571.jpg" alt="" />
          <h3>The Donut Burger</h3>
          <p>$6.99</p>
        </div>
      </div>
      <button class="btn-menu btn rounded-pill fw-bold">
        start your order <i class="fas fa-arrow-circle-right"></i>
      </button>
    </div>
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
          <img
            class="me-4"
            src="../assets/img/app-store-badge-200x67.png"
            alt="app store"
          />
          <img
            src="../assets/img/play-store-badge-200x67.png"
            alt="play store"
          />
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import Categories from "./Categories.vue";

export default {
  name: "Main",
  components: {
    Categories,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
.popular {
  padding: 5em 0;
}
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
p {
  color: $button;
}
.btn-menu {
  background-color: $button;
  text-transform: uppercase;
  color: $white;
  font-size: 0.8em;
  width: 16em;
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
