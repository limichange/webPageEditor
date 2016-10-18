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
    <webpage>
      <div class="cube"></div>
    </webpage>
  </el-col>
</el-row>
</template>

<script>
import Webpage from './WebPage.vue'

export default {
  name: 'main-edit-area',
  components: {
    Webpage
  },
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

.cube {
  width: 5rem;
  height: 5rem;
  background: #eee;
}

.slideBar {
  background: #cccccc;
}

.main-edit-area {
  background: #e5e9f2;
  height: 100%;
}

</style>
