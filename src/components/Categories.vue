<template>
  <li class="appetizers">
    <img :src="img" :alt="title" />
    <span class="d-flex justify-content-center align-items-center fw-bold">{{
      title
    }}</span>
  </li>
  <!-- <li class="burgers">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >burgers</span
      >
    </li>
    <li class="pizza">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >pizza</span
      >
    </li>
    <li class="fries">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >fries</span
      >
    </li>
    <li class="sides">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >sides</span
      >
    </li>
    <li class="desserts">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >desserts</span
      >
    </li>
    <li class="beverages">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >beverages</span
      >
    </li>
    <li class="specials">
      <span
        class="opacity d-flex justify-content-center align-items-center fw-bold"
        >specials</span
      >
    </li> -->
</template>

<script>
export default {
  name: "Categories",
  props: ["img", "title"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

li {
  height: 240px;
  width: calc((100% / 4) - 1rem);
  position: relative;
  img {
    width: 100%;
  }
  span {
    height: 100%;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    text-transform: uppercase;
    color: $white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
// .appetizers {
//   background-image: url(../assets/img/appetizers-menu-background.jpg);
// }
// .burgers {
//   background-image: url(../assets/img/burgers-menu-background.jpg);
// }
// .pizza {
//   background-image: url(../assets/img/pizza-menu-background.jpg);
// }
// .fries {
//   background-image: url(../assets/img/fries-menu-background.jpg);
// }
// .desserts {
//   background-image: url(../assets/img/sides-menu-background.jpg);
// }
// .sides {
//   background-image: url(../assets/img/desserts-menu-background.jpg);
// }
// .beverages {
//   background-image: url(../assets/img/beverages-menu-background.jpg);
// }
// .specials {
//   background-image: url(../assets/img/specials-menu-background.jpg);
// }
</style>
