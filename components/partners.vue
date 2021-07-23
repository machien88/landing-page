<template>
    <div class="partners" id="partners">
        <div class="content">
            <div class="left">
                <img src="../assets/images/partners/avatar.png">
            </div>
            <div class="right">
                <div class="sub-title">BPLAY GAME</div>
                <div class="title">PARTNERS</div>
                <div class="description">{{description}}</div>
                <div class="list-card">
                    <div class="card">
                        <img src="../assets/images/partners/sbtech.png">
                    </div>
                    <div class="card">
                        <img src="../assets/images/partners/iovation.png">
                    </div>
                    <div class="card">
                        <img src="../assets/images/partners/seon.png">
                    </div>
                    <div class="card">
                        <img src="../assets/images/partners/hogaming.png">
                    </div>
                    <div class="card">
                        <img src="../assets/images/partners/vivo.png">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data () {
    return {
      description: 'As a BPlay client you will benefit from content from more than 20 top tier providers. Based on your casino’s concept and targeted markets, we will tailor the perfect portfolio of games to offer to your players.'
    }
  }
}
</script>
<style lang="scss">
  .partners {
    @import '../assets/css/partners.scss';
  }
</style>