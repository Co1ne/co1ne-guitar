<template>
<div class="video-item">
  <el-row>
    <el-col :span="32">
      <el-card :body-style="{ padding: '0px' }">
        <img v-bind:src="poster" class="image">
        <div style="padding: 14px;" align="left">
          <span>{{title}}</span>
          <div class="bottom clearfix">
            <time class="time">{{ currentDate }}</time>
            <el-button type="text" class="button">播放</el-button>
          </div>
        </div>
      </el-card>
    </el-col>
  </el-row>
</div>
</template>
<style>
.video-item {
  min-width: 300px;
  float: left;
  width: 25%;
  display: -webkit-flex;
  -webkit-justify-content: center;
  -webkit-align-items: center;
  margin: 10px auto;
}

.time {
  font-size: 13px;
  color: #999;
}

.bottom {
  margin-top: 13px;
  line-height: 12px;
}

.button {
  padding: 0;
  float: right;
}

.image {
  width: 100%;
  display: block;
}

.clearfix:before,
.clearfix:after {
  display: table;
  content: "";
}

.clearfix:after {
  clear: both
}
</style>

<script>
export default {
  data() {
    return {
      currentDate: new Date(),
      poster: "https://f10.baidu.com/it/u=2659474507,660568095&fm=72",
      title: "我的弹唱作品"
    };
  }
}
</script>
