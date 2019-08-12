<template>
  <div>
    <div>{{msg}}</div>

    <div class="search-bar">
      <el-row>
        <el-col :span="3"><img :src="locationIcon" width="80%" class="location-icon"></el-col>
        <el-col :span="16"><input type="text" class="search-input"/></el-col>
        <el-col :span="5"><el-button size="medium">查找</el-button></el-col>
      </el-row>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data(): object {
    return {
      msg: "Shopping Mall component working!",
      locationIcon: require('../assets/17-170231_location-icons-location-png.png')
    };
  }
});
</script>

<style scoped>
.search-bar {
  height: 2.2rem;
  background-color: #e5017d;
  line-height: 2.2rem;
}
.search-input{
      width:100%;
      height: 1.3rem;
      border-top:0px;
      border-left:0px;
      border-right:0px;
      border-bottom: 1px solid 1px !important ;
      background-color: #e5017d;
      color:#fff;
  }
  .location-icon{
      padding-top: .2rem;
      padding-left: .3rem;
  }
</style>
