<template>
  <footer>
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-2">
          <ul>
            <li><h5>order online</h5></li>
            <li><a href="#">Appetizers</a></li>
            <li><a href="#">Burgers</a></li>
            <li><a href="#">Pizza</a></li>
            <li><a href="#">Fries</a></li>
            <li><a href="#">Sides</a></li>
            <li><a href="#">Desserts</a></li>
            <li><a href="#">Beverages</a></li>
            <li><a href="#">Specials</a></li>
          </ul>
        </div>
        <div class="col-2">
          <ul>
            <li><h5>navigate</h5></li>
            <li><a href="#">Home</a></li>
            <li><a href="#">Alternate Home</a></li>
            <li><a href="#">Menu</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Cart</a></li>
          </ul>
        </div>
        <div class="col-2">
          <ul>
            <li><h5>information</h5></li>
            <li><a href="#">My Account</a></li>
            <li><a href="#">Terms Of Service</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li>
              <a href="#"
                ><img
                  class="border border-2 rounded"
                  src="../assets/img/app-store-badge-200x67.png"
                  alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img
                  class="border border-2 rounded"
                  src="../assets/img/play-store-badge-200x67.png"
                  alt=""
              /></a>
            </li>
          </ul>
        </div>
        <div class="col-2">
          <ul>
            <li><h5>opening hours</h5></li>
            <li>Mon - <span>10AM to 11PM</span></li>
            <li>Tue - <span>10AM to 11PM</span></li>
            <li>Wed - <span>10AM to 11PM</span></li>
            <li>Thur - <span>10AM to 11PM</span></li>
            <li>Fri - <span>10AM to 11PM</span></li>
            <li>Sat - <span>10AM to 1AM</span></li>
            <li>Sun - <span>11AM to 10PM</span></li>
          </ul>
        </div>
        <div class="col-2">
          <ul>
            <li><h5 class="text-center">voucher</h5></li>
            <li>
              <img src="../assets/img/footer-coupon-200x200.png" alt="" />
            </li>
            <li class="text-center fw-bold fs-5">
              Just Use The Code
              <br />
              <span class="fs-3">FIRSTORDER</span>
              <br />
              At Checkout
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

footer {
  margin-top: 10em;
  height: 1100px;
  background-image: url(../assets/img/footer-background-scaled.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  .container {
    width: 90%;
    padding: 5em 0;
  }
}
li {
  color: $white;
  font-size: 0.9em;
  margin-bottom: 0.8em;
  h5 {
    text-transform: uppercase;
    margin-bottom: 1.4em;
    font-size: 1.2em;
  }
  img {
    width: 100%;
  }
  span {
    color: $yellow;
  }
}
</style>
