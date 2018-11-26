<template>
<div id="navi">
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" text-color="#000" active-text-color="#ffd04b">
    <el-menu-item index="1">
      <router-link to="/" tag="li">主页</router-link>
    </el-menu-item>
    <el-menu-item index="2">
      <router-link to="/recommand" tag="li">推荐</router-link>
    </el-menu-item>
    <el-menu-item index="3">
      <router-link to="/collaboration" tag="li">共创</router-link>
    </el-menu-item>
    <el-menu-item index="4">
      <router-link to="/course" tag="li">教学</router-link>
    </el-menu-item>

  </el-menu>
  <div class="line"></div>
</div>
</template>
<script>
export default {
  data() {
    return {
      activeIndex: '1',
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>
