<template>
  <div class="goods">
    <goods-list-item v-for="item in goods" :goods-item="item" :key="item.id" />
  </div>
</template>

<script>
import GoodsListItem from "./GoodsListItem";

export default {
  name: "",
  components: {
    GoodsListItem,
  },
  props: {
    goods: {
      type: Array,
      default() {
        return [];
      },
    },
  },
};
</script>

<style scoped>
.goods {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
</style>
