<template>
  <button class="demo-button">
    <div class="test">测试样式</div>
    <slot />
  </button>
</template>

<script lang="ts">

export default {
  name: 'DemoButton',

  props: {
    color: String,
    type: {
      type: String,
      default: 'primary',
    },
  },
};
</script>

<style lang="scss">
.demo-button {
  min-width: 120px;
  color: #fff;
  font-size: 16px;
  line-height: 36px;
  background-color: #f44;
  border: none;
  border-radius: 30px;
}
</style>
