<template>
  <div class="home">
    <!-- 导航栏 -->
    <common-bar>
      <!-- 左边插槽 -->
      <template v-slot:left>
        <el-icon><Expand /></el-icon>
      </template>
      <!-- 中间插槽 -->
      <template v-slot:middle> 
        <el-input class="input" :prefix-icon="Search"></el-input>
      </template>
      <!-- 右边插槽 -->
      <template v-slot:right> 
        <el-icon><Mic /></el-icon>
      </template>
    </common-bar>
  </div>
</template>

<script setup lang="ts">
import { ElButton,ElInput } from "element-plus";
import { Search } from '@element-plus/icons-vue'
</script>

<style lang="scss" scoped>
.input{
    width: 17rem;
  }
 .home>>>.el-input{
  border-radius: rem;
 }
</style>
