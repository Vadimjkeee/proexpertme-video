<template>
  <section class="video">
    <div class="container">
      <div class="video-wrapper">
      <h1 class="video__title">{{ title }}</h1>
        <video-list :list="list" />
      </div>
      <div class="more">
        <p class="more__text">{{ more.text}}</p>
        <img :src="more.arrow.src" :alt="more.alt" class="arrow" />
      </div>
    </div>
  </section>
</template>
  
  <script>
import VideoList from "@/components/VideoList";
export default {
  props: {
    title: { 
      type: String, 
      default: "Обучающие видео"
    },
    list: { type: Array },
  },
  components: {
    VideoList,
  },
  data() {
    return {
      more: { 
        text: 'Показать ещё',
        arrow: {
            src: require("@/assets/img/arrow.svg"), alt: " " },
      }
    };
  },
};
</script>
  
  <style scoped lang="scss">
  @import '@/assets/scss/modules/mixins.scss';
  .more {
    display: flex;
    align-items: center;
    justify-content: center;
    &__text {
        margin-right: 2rem;
        font-family: "Montserrat Bold";
        @include adaptiv-font(2.039, 1.4);
        line-height: 120%;
        color: #000000;
    }
}
.arrow {
    border: none;
    cursor: pointer;
    background-color: inherit;
}

.video {
    padding: 6rem 2rem;
    &__title {
        font-family: "Montserrat Bold";
        @include adaptiv-font(7, 4);
        line-height: 100%;
        color: #000000;
        margin-left: 11%;
        @media (max-width: 1400px) {
            text-align: center;
            margin-left: 0;
        }
    }
}

.video-wrapper{
  row-gap: 6rem;
  display: flex;
    flex-direction: column;
}


</style>