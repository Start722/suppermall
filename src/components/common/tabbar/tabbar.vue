<template>
  <div id="tabBar">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'tabbar',
}
</script>

<style>
  #tabBar{
    display: flex;
    background-color: #f6f6f6;

    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 9;

    box-shadow: 0 -1px 1px rgba(100, 100, 100, .09);
  }
</style>
