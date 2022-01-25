<template>
  <div class="container">
    <div class="row mb-5">
      <div class="col-6">
        <h2 class="fw-bold">Latest News</h2>
      </div>
      <div class="col-6 text-end">
        <button class="btn rounded-pill fw-bold">
          read more news <i class="fas fa-arrow-circle-right"></i>
        </button>
      </div>
    </div>
    <div class="row">
      <div class="col-6">
        <img src="../assets/img/pancake-burger-600x450.jpg" alt="" />
        <h3 class="text-center fw-bold">NEW: The Pancake Burger</h3>
        <p class="text-center">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi aliquid
          deserunt asperiores sed deleniti officiis repellat non libero numquam,
          alias tenetur inventore placeat quaerat soluta saepe sit error
          distinctio possimus.
        </p>
      </div>
      <div class="col-6">
        <img src="../assets/img/new-milkshake-menu-600x450.jpg" alt="" />
        <h3 class="text-center fw-bold">New Milkshake Menu</h3>
        <p class="text-center">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi aliquid
          deserunt asperiores sed deleniti officiis repellat non libero numquam,
          alias tenetur inventore placeat quaerat soluta saepe sit error
          distinctio possimus.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LatestNews",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
button {
  background-color: $button;
  text-transform: uppercase;
  color: $white;
  font-size: 0.8em;
  width: 16em;
}
</style>
