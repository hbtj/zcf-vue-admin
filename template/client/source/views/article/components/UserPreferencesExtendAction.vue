<template>
  <div class="plugin">
    <div class="panel-card">
      <h4 class="panel-legend">文章</h4>
      <el-row :gutter="20">
        <el-col :span="9"><span>全屏编辑发布后关闭窗口：</span></el-col>
        <el-col :span="15">
          <el-switch v-model="preferences.closeWindowAfterPublish" active-value="Y" inactive-value="N" ></el-switch>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  props: ['preferences']
}
</script>

<style scoped>
.plugin{
  border: 1px solid #f7f8fa;
  background-color: #f7f8fa;
}
.plugin .title{
  padding: 20px 10px 0;
}
.plugin .panel-card{
  padding: 10px;
}
</style>
