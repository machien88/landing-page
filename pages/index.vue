<template>
  <div>
    <todo-header/>
    <div class="onTop" @click="goto">
      <img src="../assets/img/header/top.png">
    </div>
  </div>
</template>

<script>
import TodoHeader from '~/components/header'

export default {
  components: {
    TodoHeader,
  },
  methods: {
    goto() {
      let element = document.getElementById('header');
      let top = element.offsetTop;
      window.scrollTo(0, top);
    }
  }
}
</script>
<style>
  .onTop {
    position: fixed;
    bottom: 10px;
    right: 0;
    z-index: 99;
    font-size: 18px;
    border: none;
    outline: none;
    color: white;
    cursor: pointer;
    padding: 15px;
  }
  .onTop img {
    width: 50px;
  }
</style>
