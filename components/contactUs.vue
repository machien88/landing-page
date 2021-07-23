<template>
  <div class="contact-us" id="contact-us">
      <div class="content">
        <div class="left">
            <img src="../assets/images/header/logo.svg">
        </div>
        <div class="right">
          <div class="content">
              <div class="contact-title">CONTACT US</div>
              <div class="address">
                <img src="../assets/images/contactUS/location.png">
                <div class="address-title">
                  2901 Marmora Road, Glassgow, 
                  Seattle,
                  WA 98122-1090
                </div>
              </div>
              <div class="address">
                <img src="../assets/images/contactUS/letter.png">
                <div class="address-title">info@bplay.com</div>
              </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {}
</script>
<style lang="scss">
  .contact-us {
    background-image: url('../assets/images/contactUS/background.png');
    background-size: cover;
    @import '../assets/css/contactUs.scss';
  }
</style>
