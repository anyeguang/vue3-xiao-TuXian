<script setup lang="ts">
import request from './utils/request';
import { onMounted } from 'vue';

onMounted(async () => {
  const res = await request.get('/home/index');
  console.log(res);
});
</script>

<template>
  <h1>Vue3+TS小兔鲜儿</h1>
</template>
<style lang="less" scoped>
// 必须导入 variables.less
@import '@/assets/styles/variables.less';
@import '@/assets/styles/mixins.less';
h1 {
  background-color: @warnColor;
  .hoverShadow();
}
</style>
