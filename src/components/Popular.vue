<template>
  <div class="col-4">
    <img :src="img" :alt="name" />
    <h3>{{ name }}</h3>
    <p>{{ price }}</p>
  </div>
  <!-- <div class="col-4">
        <img src="../assets/img/choco-cookie-frappe-400x571.jpg" alt="" />
        <h3>Choko Cookie Frappe</h3>
        <p>$4.99</p>
      </div>
      <div class="col-4">
        <img src="../assets/img/donut-burger-400x571.jpg" alt="" />
        <h3>The Donut Burger</h3>
        <p>$6.99</p>
      </div> -->
</template>

<script>
export default {
  name: "Popular",
  props: ["img", "name", "price"],
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

p {
  color: $button;
}
</style>
