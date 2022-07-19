<template>
  <iframe :src="src" scrolling="auto" frameborder="0" />
</template>

<script setup lang="ts">
defineProps<{
  src: string
}>()
</script>
<style lang="less" scoped>
iframe {
  min-height: calc(100vh - var(--header-height) - var(--footer-height));
}
</style>
