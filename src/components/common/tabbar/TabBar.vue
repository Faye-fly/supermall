<template>
  <div id="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'tabbar',
  components: {},
}
</script>

<style>
@import 'assets/css/base.css';

#tab-bar {
  display: flex;
  height: 49px;

  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #f6f6f6;
  box-shadow: 0 -1px 1px rgba(1, 1, 1, 0.08);
}
</style>
