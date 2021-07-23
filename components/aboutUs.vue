<template>
    <div class="about-us" id="about-us">
        <div class="content">
            <div class="sub-title">BPLAY GAME</div>
            <div class="title">WHO WE ARE?</div>
            <div class="title-body">{{titleBody}}</div>
        </div>
        <div class="content-image">
            <img class="map" src="../assets/images/aboutUS/content.png">
            <img class="location" src="../assets/images/aboutUS/sub-content.png">
            <div class="content building">
                <div class="sub-content"></div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data () {
    return {
      titleBody: 'BPlay was founded in 2015 by a group of highly skilled professionals with over 15 years of experience in the iGaming industry. Today we are an international company with more than 100 employees and have operations in Malta, Ukraine, Romania, Norway, India, Myanmar and Taiwan...'
    }
  }
}
</script>
<style lang="scss">
  .about-us {
    @import '../assets/css/aboutUs.scss';
  }
</style>