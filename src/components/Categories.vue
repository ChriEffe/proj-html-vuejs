<template>
  <div class="categories container">
    <div class="row mb-4">
      <div class="col-6">
        <h2 class="fw-bold">Menu Categories</h2>
      </div>
      <div class="col-6 text-end">
        <button class="btn rounded-pill fw-bold">
          view the full menu <i class="fas fa-arrow-circle-right"></i>
        </button>
      </div>
    </div>
    <ul class="d-flex flex-wrap gap-3">
      <li class="appetizers">
        <span
          class="opacity d-flex justify-content-center align-items-center fw-bold"
          >appetizers</span
        >
      </li>
      <li class="burgers">
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
      </li>
      <li class="d-flex justify-content-center align-items-center">
        <img src="../assets/img/vegetarian-icon.png" alt="" />
      </li>
      <li class="d-flex justify-content-center align-items-center">
        <img class="w-50" src="../assets/img/gluten-free-icon.png" alt="" />
      </li>
      <li class="d-flex justify-content-center align-items-center">
        <img src="../assets/img/dairy-free-icon.png" alt="" />
      </li>
      <li class="d-flex justify-content-center align-items-center">
        <img src="../assets/img/keto-friendly-icon.png" alt="" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Categories",
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
li {
  height: 240px;
  width: calc((100% / 4) - 1rem);
  background-size: contain;
  background-repeat: no-repeat;
  span {
    display: block;
    height: 100%;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    text-transform: uppercase;
    color: $white;
  }
  img {
    width: 40%;
  }
}
.appetizers {
  background-image: url(../assets/img/appetizers-menu-background.jpg);
}
.burgers {
  background-image: url(../assets/img/burgers-menu-background.jpg);
}
.pizza {
  background-image: url(../assets/img/pizza-menu-background.jpg);
}
.fries {
  background-image: url(../assets/img/fries-menu-background.jpg);
}
.desserts {
  background-image: url(../assets/img/sides-menu-background.jpg);
}
.sides {
  background-image: url(../assets/img/desserts-menu-background.jpg);
}
.beverages {
  background-image: url(../assets/img/beverages-menu-background.jpg);
}
.specials {
  background-image: url(../assets/img/specials-menu-background.jpg);
}
</style>
