<template>
  <header class="p-relative">
    <button class="add btn rounded-circle">+</button>
    <div class="container">
      <!-- navbar -->
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
      <div class="content">
        <h4 class="fs-1">Hungry?</h4>
        <h1>
          <span>Great Food</span>
          <br />
          Delivered
        </h1>
        <button class="btn-menu btn rounded-pill fw-bold">
          view our menu <i class="fas fa-arrow-circle-right"></i>
        </button>
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
  .add {
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
  .btn-menu {
    background-color: $button;
    text-transform: uppercase;
    color: $white;
    font-size: 0.8em;
    margin-top: 1.5em;
  }
}
</style>
