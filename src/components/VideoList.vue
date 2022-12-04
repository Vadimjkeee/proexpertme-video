<template>
  <div class="list">
    <video-item :key="item.id" v-for="item in list" :item="item" />
  </div>
</template>
    
<script>
import VideoItem from "@/components/VideoItem";
export default {
  props: {
    list: { type: Array },
  },
  components: { VideoItem },
  data() {
    return {};
  },
};
</script>
    
<style scoped lang="scss">
.list {
  column-gap: 2rem;
  row-gap: 3rem;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  @media (max-width: 1023px) {
    justify-content: center;
  }
}
</style>