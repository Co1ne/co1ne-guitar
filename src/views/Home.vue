<template>
<div class="home">
  <div class="home-container">
    <VideoItem/>
    <VideoItem/>
    <VideoItem/>
    <VideoItem/>
    <VideoItem/>
    <VideoItem/>
    <VideoItem/>
  </div>
  <el-pagination layout="prev, pager, next" :total="50" style="float:right;margin:2em">
  </el-pagination>
</div>
</template>
<script>
import VideoItem from '../components/VideoItem'
export default {
  name: 'home',
  components: {
    VideoItem
  }
}
</script>
<style>
.home {}

.home-container {
  width: 100%;
  height: 60%;
  overflow: auto;
  max-height: 1000px;
}
</style>
