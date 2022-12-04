<template>
  <div class="app">
    <section-video :title="title" :list="list" />
  </div>
</template>

<script>
import SectionVideo from "@/components/SectionVideo";
export default {
  components: { SectionVideo },
  data() {
    return {
      title: "Обучающие видео",
      list: [
        {
          image: { src: require("@/assets/img/doctors.png"), alt: "Доктора" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/child.png"), alt: "Мальчик" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Инновация: La Roche-Posay Vitamin 10 Антиоксидантная сыворотка для обновления кожи',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/baby.png"), alt: "Ребенок" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/woman.png"), alt: "Женщина" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Инновация: La Roche-Posay Vitamin 10 Антиоксидантная сыворотка для обновления кожи',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/child.png"), alt: "Мальчик" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Инновация: La Roche-Posay Vitamin 10 Антиоксидантная сыворотка для обновления кожи',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/doctors.png"), alt: "Доктора" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/woman.png"), alt: "Женщина" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк"},
          title: 'Инновация: La Roche-Posay Vitamin 10 Антиоксидантная сыворотка для обновления кожи',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/baby.png"), alt: "Ребенок" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк"},
          title: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/doctors.png"), alt: "Доктора" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Первая международная онлайн-конференция «Как бороться со стрессом и тревогой?»',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
        {
          image: { src: require("@/assets/img/child.png"), alt: "Мальчик" },
          play: { src: require("@/assets/img/play.svg"), alt: "Воспроизвести" },
          like: { src: require("@/assets/img/like.svg"), alt: "Лайк" },
          title: 'Инновация: La Roche-Posay Vitamin 10 Антиоксидантная сыворотка для обновления кожи',
          video: { src: "https://htmlbase.ru/storage/app/media/demo.mp4" }
        },
      ],
    };
  },
};
</script>

<style>
</style>