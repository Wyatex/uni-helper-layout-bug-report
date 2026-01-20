<script setup lang="ts">
import { isH5, isMpWeixin } from '@uni-helper/uni-env'

definePage(() => {
  const title = isH5 ? 'H5 环境' : isMpWeixin ? '微信小程序 环境' : '其他 环境'
  return {
    title,
    type: 'home',
    layout: isH5 ? 'home' : 'default',
  }
})
</script>

<template>
  <AppLogos />
  <InputEntry />
</template>

<style></style>
