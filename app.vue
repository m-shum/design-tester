<script setup lang="ts">
useBreakpoints()
</script>
<template>
  <UtilsGrid />
  <ClientOnly>
    <UtilsControls />
  </ClientOnly>
  <main class="container">
    <SampleCopy />
  </main>
</template>
<style lang="scss">
.test {
  color: red;

  /* background: black; */
  display: flex;
  gap: var(--gutter);

  @include use-mq('min-xl') {
    color: black;
  }
}
</style>
