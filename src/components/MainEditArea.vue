<template>
<el-row class="main-edit-area">
  <el-col :span="4" class="slideBar">
    <el-row>
      <el-col :span="24">
        <el-button>Tool</el-button>
        <el-slider max="64" v-model="value2"></el-slider>
        <input type="color" value="#ff0000" />
      </el-col>
    </el-row>
  </el-col>
  <el-col :span="20" >
    <div class="webpage-c">
      <div class="webpage">
        <div class="cube"></div>
      </div>
    </div>
  </el-col>
</el-row>
</template>

<script>
export default {
  name: 'main-edit-area',
  data () {
    return {
      value2: 64
    }
  },
  watch: {
    value2 (value) {
      document.documentElement.style.fontSize = `${value}px`
    }
  },
  ready () {

  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>

.slideBar {
  background: #cccccc;
}

.main-edit-area {
  background: #e5e9f2;
  height: 100%;
}

.webpage-c {
  margin: 0 auto;
  width: 10rem;
  height: 16.1rem;

  .webpage {

    .cube {
      width: 5rem;
      height: 5rem;
      background: #eee;
    }

    width: 10rem;
    height: 16.1rem;
    background: #13CE66;
  }
}

</style>
