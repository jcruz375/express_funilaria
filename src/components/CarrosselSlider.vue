<template>
  <swiper
    :modules="modules"
    :slides-per-view="1"
    :space-between="25"
    navigation
    loop
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <SwiperSlide>
      <img
        src="../../public/assets/carro-4.jpg"
        alt="Imagem de um carro sendo reparado na oficina Funilaria Express"
      />
    </SwiperSlide>
    <SwiperSlide>
      <img
        src="../../public/assets/carro-3.jpg"
        alt="Imagem de um carro sendo reparado na oficina Funilaria Express"
      />
    </SwiperSlide>
    <SwiperSlide>
      <img
        src="../../public/assets/carro-2.jpg"
        alt="Imagem de um carro sendo reparado na oficina Funilaria Express"
      />
    </SwiperSlide>
  </swiper>
</template>
<script>
import { Navigation, Pagination, Scrollbar, A11y } from "swiper/modules";

import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css/bundle";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log("slide change");
    };
    return {
      onSwiper,
      onSlideChange,
      modules: [Navigation, Pagination, Scrollbar, A11y],
    };
  },
};
</script>

<style lang="scss" scoped>
img {
  max-width: 500px;
  max-height: 500px;
  display: block;
  margin: 0 auto;
}

@media (max-width: 768px) {
  img {
    max-width: 320px;
  }
}
</style>