<template>
  <div id="app">
    <TabBar></TabBar>
    <router-view></router-view>
  </div>
</template>

<script>
  import TabBar from '@/components/common/tabbar/TabBar'
  export default {
    name: '',
    data() {
      return {

      }
    },git
    components: {TabBar}
  }
</script>


<style>
  @import "/assets/css/base.css";


</style>
