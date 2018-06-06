<template>
  <div class="container">
    This is home page!! welcome~
    <button @click="$store.commit('increment')">{{$store.state.counter}}</button>
    <a-button type="primary">Primary</a-button>
    <a-button>Default</a-button>
    <a-button type="dashed">Dashed</a-button>
    <a-button type="danger">Danger</a-button>
  </div>
</template>


<script>
import Vue from 'vue'
import {Button} from 'vue-antd-ui' // 模块的style属性可以做到按需自动加载
import '~/static/style/variable.less'
Vue.component(Button.name, Button)
  export default {
    name: '',
  }
</script>

<style scoped>

</style>