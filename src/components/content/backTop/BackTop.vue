<template>
  <div class="back-top" @click="backClick">
    <img src="~assets/img/common/top.png" alt="" />
  </div>
</template>

<script>
export default {
  methods: {
    backClick() {
      console.log('回到顶部')
    },
  },
}
</script>

<style>
.back-top {
  position: fixed;
  right: 6px;
  bottom: 50px;
}

.back-top img {
  width: 43px;
}
</style>
