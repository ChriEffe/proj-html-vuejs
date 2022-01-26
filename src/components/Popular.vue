<template>
  <div class="col-4">
    <div class="p-relative">
      <img :src="img" :alt="name" />
      <div class="display-n">
        <span
          class="add-cart d-flex flex-column justify-content-center align-items-center"
          ><button class="btn rounded-circle">
            <i class="fs-2 far fa-check-square"></i></button
          >view cart</span
        >
      </div>
    </div>
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
.p-relative {
  position: relative;
  img {
    width: 100%;
  }
  .display-n {
    display: none;
    .add-cart {
      height: 100%;
      width: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      text-transform: uppercase;
      color: $white;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      display: none;
    }
  }
  .display-n:hover {
    display: block;
  }
}
button {
  background-color: rgba(0, 0, 0, 0.8);
  padding: 1em 1.2em;
  color: white;
}
</style>
