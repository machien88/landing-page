<template>
  <div class="products" id="products">
    <img class="background" src="../assets/images/products/backgroud.png" />
    <div class="content">
      <div class="left">
        <div class="sub-title">BPLAY GAME</div>
        <div class="title">OUR PRODUCTS</div>
      </div>
      <div class="paragrap">{{description}}</div>
    </div>
    <div class="list">
      <div class="card">
        <img src="../assets/images/products/casino-live.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/fishing-game.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/sport-book.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/number-game.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/white-label.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/slots.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/api.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/package.png" />
      </div>
      <div class="card">
        <img src="../assets/images/products/table.png" />
      </div>
    </div>
    <div class="slides-mobile">
      <VueSlickCarousel :dots="true" :arrows="false">
        <div class="card">
          <img src="../assets/images/products/casino-live.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/fishing-game.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/sport-book.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/number-game.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/white-label.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/slots.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/api.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/package.png" />
        </div>
        <div class="card">
          <img src="../assets/images/products/table.png" />
        </div>
      </VueSlickCarousel>
    </div>
  </div>
</template>
<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  name: "MyComponent",
  components: { VueSlickCarousel },
  data() {
    return {
      description:' BPlay’s high quality iGaming Platform offers a complete solution for your casino. Get the full White Label turnkey solution or the Seamless API with our comprehensive selection of games. Through our global network of premium partners such as Vivo Gaming, SBTech and HoGaming you will have access to the best Live Casino, Sportsbook, Slots, Table Games, Number Games and Fishing Games on the market.'   
       };
  },
};
</script>
<style lang="scss">
.products {
  background-image: url("../assets/images/products/backroud-wave.png");
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  padding-bottom: 200px;
  @media (max-width: 385px) {
    padding-bottom: 0;
  }
  @import "../assets/css/products.scss";
}
</style>