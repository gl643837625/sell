<template>
  <div id="app">
    <v_header></v_header>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/goods">商品</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/ratings">评论</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/seller">商家</router-link>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import header from './components/header/header'

export default {
  name: 'App',
  components: {
    v_header: header
  }
}
</script>

<style lang="less" rel="stylesheet/stylus">
  #app {
    .tab {
      display: flex;
      width: 100%;
      height: 40px;
      line-height: 40px;

      .tab-item {
        flex: 1;
        text-align: center;
      }
    }
  }
</style>
