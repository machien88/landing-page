<template>
  <header class="header" id="header">
    <div class="container-fluid">
      <nav class="navbar navbar-inverse">
        <div class="header-logo">
          <img src="../assets/img/header/logo.svg">
        </div>
        <div class="container-fluid">
          <ul class="nav navbar-nav">
            <li><a id="len1" class="hoverable nav-item" @click="goto('about-us')">ABOUT US</a></li>
            <li><a id="len2" class="hoverable nav-item" @click="goto('products')">PRODUCTS</a></li>
            <li><a id="len3" class="hoverable nav-item" @click="goto('partners')">PARTNERS</a></li>
            <li><a id="len4" class="hoverable nav-item" @click="goto('our-clients')">OUR CLIENTS</a></li>
            <li><a id="len5" class="hoverable nav-item" @click="goto('contact-us')">CONTACT US</a></li>
          </ul>
        </div>
        <div class="header-lang">
          <select class="form-control lang" id="language">
            <option value="ENG">ENG</option>
            <option value="VNE">VNE</option>
          </select>
        </div>
        <div class="menubtn mobile" @click="openMenu">
          <img src="../assets/img/header/menu.png">
        </div>
      </nav>
    </div>
    <div class="home-page">
      <div class="title">CASINO PLAY GAME</div>
    </div>
    <div class="overlay" v-if="isOpen"></div>
    <div class="modal" v-if="isOpen">
      <div class="control">
        <div class="lang-mobile">
          <select class="form-control lang" id="language">
            <option value="ENG">ENG</option>
            <option value="VNE">VNE</option>
          </select>
        </div>
        <div class="close-btn" @click="closeMenu">X</div>
      </div>
      <div class="nav-mobile">
        <div class="item"><a id="len1" @click="goto('about-us')">ABOUT US</a></div>
        <div class="item"><a id="len2" @click="goto('products')">PRODUCTS</a></div>
        <div class="item"><a id="len3" @click="goto('partners')">PARTNERS</a></div>
        <div class="item"><a id="len4" @click="goto('our-clients')">OUR CLIENTS</a></div>
        <div class="item"><a id="len5" @click="goto('contact-us')">CONTACT US</a></div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data () {
    return {
      isOpen: false
    }
  },
  methods: {
    openMenu () {
      this.isOpen = true;
      document.body.style.overflow = "hidden";
    },
    closeMenu () {
      this.isOpen = false;
      document.body.style.overflow = "auto";
    },
    goto(id) {
      this.isOpen = false;
      let element = document.getElementById(id);
      let top = element.offsetTop;
      window.scrollTo(0, top);
    }
  }
}
</script>
<style lang="scss">
  .header {
    background-image: url('../assets/img/header/banner.png');
    background-size: cover;
    @media (max-width: 385px) {
      height: 40vh;
    }
    @import '../assets/css/header.scss';
  }
</style>
