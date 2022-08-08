<template>
<!-- 公共三栏布局，两边固定，中间自适应 -->
<div class="common-bar">
  <!-- 左边 -->
  <div class="common-bar-left">
    <slot name="left"></slot>
  </div>
  <!-- 中间 -->
  <div class="common-bar-middle">
    <slot name="middle"></slot>
  </div>
  <!-- 右边 -->
  <div class="common-bar-right">
    <slot name="right"></slot>
  </div>
</div>
</template>

<script setup>
import {} from 'vue'
</script>

<style lang="scss" scoped>
.common-bar{
  display: flex;
  align-items: center;
  justify-content: space-between;
  .common-bar-left,.common-bar-right{
    width: 2rem;
    height: 2rem;
    display: flex;
    align-items: center;
    font-size: 1.5rem;
  }
  .common-bar-right{
    justify-content: end;
  }
  .common-bar-middle{
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
}

</style>