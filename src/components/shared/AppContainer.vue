<template>
  <div class="container">
    <slot>Default value</slot>
  </div>
</template>

<script>
export default {
  name: "AppContainer",
};
</script>

<style lang="scss" scoped>
.container {
  max-width: 1440px;
  margin: 0 auto;
}
</style>
