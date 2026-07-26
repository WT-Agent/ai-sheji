<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了金融 APP 首页深色拟态 UI 布局设计"
  },
  {
    "text": "用户 189****9900 生成了 Midjourney 3D 盲盒公仔高清提示词"
  },
  {
    "text": "用户 131****4422 完成了 B 端 SaaS 系统配色与 Design System"
  },
  {
    "text": "用户 156****7788 生成了电商双十一预热 Banner 排版大纲"
  },
  {
    "text": "用户 177****3311 取得了网页响应式微交互动画触发说明"
  }
]);
</script>
