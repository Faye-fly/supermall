<template>
  <div class="recommend">
    <div v-for="item in recommends">
      <a :href="item.link">
        <img :src="item.image" />
        <div>{{ item.title }}</div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    recommends: {
      type: Array,
      default() {
        return []
      },
    },
  },
}
</script>

<style>
.recommend {
  display: flex;
  width: 100%;
  text-align: center;
  font-size: 12px;

  padding: 10px 0 20px;
  border-bottom: 8px solid #eee;
}

.recommend div {
  flex: 1;
}
.recommend div img {
  height: 70px;
  width: 70px;
  margin-bottom: 10px;
}
</style>
