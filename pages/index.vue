<template>
  <div>
    <todo-header/>
    <todo-aboutUs/>
    <todo-products/>
    <todo-partners/>
    <todo-ourClients/>
    <todo-contactUs/>
    <todo-footer/>
    <div class="scrollTop" @click="navigate">
      <img src="../assets/images/header/scroll-top.png">
    </div>
  </div>
</template>

<script>
import TodoHeader from '~/components/header'
import TodoAboutUs from '~/components/aboutUs'
import TodoProducts from '~/components/products'
import TodoPartners from '~/components/partners'
import TodoOurClients from '~/components/ourClients'
import TodoContactUs from '~/components/contactUs'
import TodoFooter from '~/components/footer'

export default {
  components: {
    TodoHeader,
    TodoAboutUs,
    TodoProducts,
    TodoPartners,
    TodoOurClients,
    TodoContactUs,
    TodoFooter,
  },
  methods: {
    navigate() {
      let element = document.getElementById('header');
      let top = element.offsetTop;
      window.scrollTo(0, top);
    }
  }
}
</script>
<style>
  .scrollTop {
    position: fixed;
    bottom: 15px;
    right: 0;
    z-index: 99;
    font-size: 18px;
    border: none;
    outline: none;
    color: white;
    cursor: pointer;
    padding: 15px;
  }
  .scrollTop img {
    width: 40px;
  }
</style>
