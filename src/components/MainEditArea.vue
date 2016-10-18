<template>
<el-row class="main-edit-area">
  <el-col :span="4" >
    <el-row>
      <el-col :span="24">
        <el-button>按钮1</el-button>
      </el-col>
    </el-row>
  </el-col>
  <el-col :span="20" >
    <div class="webpage-c">
      <div class="webpage"></div>
    </div>
  </el-col>
</el-row>
</template>

<script>
export default {
  name: 'main-edit-area',
  data () {
    return {

    }
  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>

.main-edit-area {
  background: #e5e9f2;
  height: 100%;
}

.webpage-c {
  margin: 0 auto;
  width: 640px;
  height: 1030px;

  .webpage {
    width: (640 / 2)px;
    height: (1030 / 2)px;
    background: #13CE66;
  }
}

</style>
