<script setup lang="ts">
import { isH5 } from '@uni-helper/uni-env'
definePage(() => {
  const title = isH5 ? 'H5 环境' : '非 H5 环境'
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
