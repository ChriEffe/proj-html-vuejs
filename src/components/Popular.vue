<template>
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
</template>

<script>
export default {
  name: "Popular",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

.popular {
  padding: 5em 0;
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
</style>
