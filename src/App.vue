<template>
<div id="app">
  <el-container>
    <el-header id="head-navi">
      <Navi/>
    </el-header>
    <el-main>
      <router-view/>
    </el-main>
    <el-footer height="200px">
      <Footer/>
    </el-footer>
  </el-container>
</div>
</template>
<script>
import Navi from './components/Navi.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'app',
  components: {
    Navi,
    Footer
  }
}
</script>
<style>
#head-navi {
  padding: 0px 0px;
}

.el-footer {
  background-color: #E9EEF3;
  color: #333;
}

.el-main {
  background-color: #f7fbfd;
  color: #333;
  text-align: center;
  line-height: 600px;
}

body>.el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
