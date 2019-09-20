<template>
  <div id="home">
    <nav-bar class="home-nav">
      <div slot="center">购物街</div>
    </nav-bar>
    <h1>首页</h1>
  </div>
</template>

<script>
  import NavBar from '@/components/common/nvabar/NavBar'
export default {
  name: '',
  data() {
    return {

    }
  },
  components: {NavBar}
}
</script>

<style scoped>
  .home-nav{
    background-color: var(--color-tint);
    color: #fff;
  }
</style>
