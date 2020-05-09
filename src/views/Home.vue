<template>
  <div class="home">
    <img class="img" alt="Vue logo" src="../assets/logo.png" />
    <div class="button">
      <span style="margin-right:20px">这是span1</span>
      <XButton @click="btnClcik" class="btnstyle">按钮</XButton>
      <span style="border:1px solid #000;margin-left:20px">这是span2</span>
    </div>

    <div class="switch">
      <XSwitch></XSwitch>
    </div>
  </div>
</template>

<script>
import XButton from '@c/button/index.vue'
import XSwitch from '@c/switch/index.vue'
export default {
  name: 'Home',
  components: { XButton, XSwitch },
  methods: {
    btnClcik() {
      console.log('父组件里面点击了按钮方法')
    }
  }
}
</script>


<style lang="less" scoped>
.img {
  display: block;
  margin: 0 auto;
}
.btnstyle {
  width: 100px;
  height: 100px;
  border: 1px solid #000;
  font-size: 20px;
}
</style>
