<template>
  <div class="tab-control">
    <div v-for="(item, index) in titles" class="tab-control-item" :class="{ active: index === currentActive }" @click="itemClick(index)">
      <span>{{ item }}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    titles: {
      type: Array,
      default() {
        return []
      },
    },
  },
  data() {
    return {
      currentActive: 0,
    }
  },
  methods: {
    itemClick(index) {
      this.currentActive = index
      this.$emit('tabClick', index)
    },
  },
}
</script>

<style scoped>
.tab-control {
  display: flex;
  font-size: 15px;
  text-align: center;
  height: 40px;
  line-height: 40px;
  background-color: #fff;
}

.tab-control-item {
  flex: 1;
}

.tab-control-item span {
  padding: 5px;
}

.active {
  color: var(--color-high-text);
}

.active span {
  border-bottom: 3px solid var(--color-tint);
}
</style>
