<template>
  <header class="p-relative">
    <button class="btn">+</button>
    <div class="container">
      <div class="row">
        <div class="col-4">
          <img class="logo" src="../assets/img/takeout-logo.png" alt="logo" />
        </div>
        <div class="col-7">
          <ul
            class="d-flex justify-content-end align-items-center h-100 fw-bold gap-5"
          >
            <li>
              <a href="#">Home <i class="fas fa-chevron-down"></i></a>
            </li>
            <li><a href="#">Order Online</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">Contact Us</a></li>
            <li>
              <a href="#"><i class="fas fa-shopping-cart"></i></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

header {
  height: 850px;
  background-image: url(../assets/img/home-background-hero-scaled.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  button {
    position: absolute;
    top: 10px;
    right: 15px;
    background-color: $button;
    color: $white;
  }
  .container .row {
    padding: 4em 0;
  }
}
</style>
