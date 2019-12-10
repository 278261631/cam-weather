<template>
  <div id="app">
    <div class="line"></div>
    <el-menu  class="el-menu-demo" mode="horizontal"
       background-color="#545c64" text-color="#fff"
      active-text-color="#ffd04b">
      <el-menu-item index="1">天气</el-menu-item>
    </el-menu>

    <div class="demo-image__preview">
      <el-image style="width: 100px; height: 100px" :src="url" :preview-src-list="srcList"> </el-image>
    </div>


    <div>
      <el-button @click="">Start</el-button>
    </div>
  </div>
</template>

<script>
export default {
 data() {
    return {
      url: 'http://www.xjltp.com/xmoon/img/xmoon1gaoyazi/allsky174.jpg',
      srcList: [
        'http://www.xjltp.com/xmoon/img/xmoon1gaoyazi/allsky174.jpg'
      ]
    }
  },
  methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
</style>
