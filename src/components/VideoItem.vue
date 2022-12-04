<template>
  <div class="video-item">
    <img
      :src="item.image.src"
      :alt="item.image.alt"
      class="preview"
      :class="{ deActive: isActive }"
    />
    <video
      class="movie"
      :class="{ active: isActive }"
      :src="item.video.src"
      autoplay
    ></video>
    <button type="submit" class="submit" :class="{ deActive: isActive }">
      <img
        :src="item.play.src"
        :alt="item.play.alt"
        class="play"
        @click="playVideo"
      />
    </button>
    <div class="like-wrapper" :class="{ deActive: isActive }">
      <img :src="item.like.src" :alt="item.like.alt" class="like" />
    </div>
    <h3 class="title">{{ item.title }}</h3>
  </div>
</template>
    
      <script>
export default {
  props: {
    item: {
      image: { type: Object, default: { src: require("@/assets/img/doctors.png"), alt: 'Доктора' }},
      video: { type: Object, default: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }},
      title: { type: String, default: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»' },
    },
  },
  data() {
    return { isActive: false };
  },
  methods: {
    playVideo() { this.isActive = true },
  },
};
</script>
      
<style scoped lang="scss">
@import "@/assets/scss/modules/mixins.scss";

.movie {
  display: none;
}

.active {
  display: inline;
}

.deActive {
  display: none;
}

.movie {
  width: 100%;
}
.title {
  padding: 2rem;
  font-family: "Montserrat Medium";
  @include adaptiv-font(2, 1.4);
  line-height: 24px;
  color: #000000;
}

.submit {
  position: absolute;
  top: 25%;
  right: 40%;
  background-color: inherit;
  border: none;
  @media (max-width: 767px) {
    top: 18%;
    right: 36%;
  }
  @media (max-width: 576px) {
    top: 13%;
    right: 31%;
  }
  @media (max-width: 480px) {
    top: 0%;
    right: 25%;
  }
}

.like-wrapper {
  position: absolute;
  top: -3%;
  right: -1%;
  @media (max-width: 480px) {
    top: -4%;
    right: -5%;
  }
}

.video-item {
  position: relative;
  max-width: 64rem;
  width: 100%;
}

.preview {
  width: 100%;
}
</style>