<template>
<div class="webpage-c">
  <div class="webpage">
    <slot></slot>
  </div>
</div>
</template>

<script>
export default {
  name: 'webpage',
  data () {
    return {

    }
  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>
.webpage-c {
  margin: 0 auto;
  width: 10rem;
  height: 16.1rem;

  .webpage {
    width: 10rem;
    height: 16.1rem;
    background: #13CE66;
  }
}
</style>
