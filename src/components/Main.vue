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
      <div class="row">
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
    <!-- offer -->
    <div class="offer"></div>
  </main>
</template>

<script>
export default {};
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
  margin-top: 1.5em;
  width: 16em;
}
.offer {
  height: 430px;
  background-image: url(../assets/img/first-order-background-scaled.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
