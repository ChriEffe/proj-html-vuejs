<template>
  <main>
    <div class="container">
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
    <div class="popular container text-center">
      <h2 class="fw-bold">Our Most Popular Dishes</h2>
      <div class="row">
        <col-4></col-4>
        <col-4></col-4>
        <col-4></col-4>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
.popular {
  padding-top: 5em;
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
</style>
