<template>
  <main>
    <div class="container">
      <!-- shop info -->
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
    <!-- popular dishes -->
    <div class="popular container text-center">
      <h2 class="fw-bold">Our Most Popular Dishes</h2>
      <div class="row mb-4">
        <Popular
          v-for="(product, index) in products"
          :key="index"
          :img="getImg(product.img)"
          :name="product.name"
          :price="product.price"
        />
      </div>
      <button class="btn-menu-p btn rounded-pill fw-bold">
        start your order <i class="fas fa-arrow-circle-right"></i>
      </button>
    </div>
    <!-- banner offer -->
    <div class="banner offer">
      <img class="wave" src="../assets/img/wave.svg" alt="" />
    </div>
    <!-- categories -->
    <div class="categories container">
      <div class="row mb-4">
        <div class="col-6">
          <h2 class="fw-bold">Menu Categories</h2>
        </div>
        <div class="col-6 text-end">
          <button class="cat- btn rounded-pill fw-bold">
            view the full menu <i class="fas fa-arrow-circle-right"></i>
          </button>
        </div>
      </div>
      <ul class="d-flex flex-wrap gap-3">
        <Categories
          v-for="(menu, index) in categories"
          :key="index"
          :img="getImg(menu.img)"
          :alt="menu.title"
          :title="menu.title"
        />
        <li
          class="allergens-icon d-flex flex-column justify-content-center align-items-center fw-bold"
        >
          <img
            class="allergens"
            src="../assets/img/vegetarian-icon.png"
            alt=""
          />
          Vegetarian
        </li>
        <li
          class="allergens-icon d-flex flex-column justify-content-center align-items-center fw-bold"
        >
          <img
            class="w-50 mb-0"
            src="../assets/img/gluten-free-icon.png"
            alt=""
          />
          Gluten Free
        </li>
        <li
          class="allergens-icon d-flex flex-column justify-content-center align-items-center fw-bold"
        >
          <img
            class="allergens"
            src="../assets/img/dairy-free-icon.png"
            alt=""
          />
          Dairy Free
        </li>
        <li
          class="allergens-icon d-flex flex-column justify-content-center align-items-center fw-bold fw-bold"
        >
          <img
            class="allergens"
            src="../assets/img/keto-friendly-icon.png"
            alt=""
          />
          Keto Friendly
        </li>
      </ul>
    </div>
    <!-- banner app -->
    <div class="banner app">
      <div class="container">
        <div class="content">
          <h4 class="fs-1">Download Our</h4>
          <h1 class="mb-5">
            <span>Ordering App</span>
          </h1>
          <a href="#"
            ><img
              class="me-4"
              src="../assets/img/app-store-badge-200x67.png"
              alt="app store"
          /></a>
          <a href="#"
            ><img
              src="../assets/img/play-store-badge-200x67.png"
              alt="play store"
          /></a>
        </div>
      </div>
    </div>
    <!-- latest news -->
    <LatestNews />
  </main>
</template>

<script>
import Categories from "./Categories.vue";
import Popular from "./Popular.vue";
import LatestNews from "./LatestNews.vue";

export default {
  name: "Main",
  components: {
    Categories,
    Popular,
    LatestNews,
  },
  data() {
    return {
      products: [
        {
          img: "img/skin-on-fries-400x571.jpg",
          name: "Skin On Fries",
          price: "$3.00-$6.00",
        },
        {
          img: "img/choco-cookie-frappe-400x571.jpg",
          name: "Choko Cookie Frappe",
          price: "$4.99",
        },
        {
          img: "img/donut-burger-400x571.jpg",
          name: "The Donut Burger",
          price: "$6.99",
        },
      ],
      categories: [
        {
          img: "img/appetizers-menu-background.jpg",
          title: "appetizers",
        },
        {
          img: "img/burgers-menu-background.jpg",
          title: "burgers",
        },
        {
          img: "img/pizza-menu-background.jpg",
          title: "pizza",
        },
        {
          img: "img/fries-menu-background.jpg",
          title: "fries",
        },
        {
          img: "img/sides-menu-background.jpg",
          title: "sides",
        },
        {
          img: "img/desserts-menu-background.jpg",
          title: "desserts",
        },
        {
          img: "img/beverages-menu-background.jpg",
          title: "beverages",
        },
        {
          img: "img/specials-menu-background.jpg",
          title: "specials",
        },
      ],
    };
  },
  methods: {
    getImg(pic) {
      return require("../assets/" + pic);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

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
.popular {
  padding: 5em 0;
}
.btn-menu-p {
  background-color: $button;
  text-transform: uppercase;
  color: $white;
  font-size: 0.8em;
  width: 16em;
}
.banner {
  height: 430px;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 5em;
}
.offer {
  background-image: url(../assets/img/first-order-background-scaled.jpg);
}
.app {
  background-image: url(../assets/img/app-ordering-scaled.jpg);
}
.cat- {
  background-color: $button;
  text-transform: uppercase;
  color: $white;
  font-size: 0.8em;
  width: 16em;
}
.allergens-icon {
  height: 240px;
  width: calc((100% / 4) - 1rem);
  .allergens {
    width: 40%;
    margin-bottom: 1.5em;
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
}
</style>
