<template>
    <swiper
    :style="{
      '--swiper-navigation-color': '#fff',
      '--swiper-pagination-color': '#fff',
    }"
    :zoom="true"
    :navigation="true"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
      <div class="swiper-zoom-container">
        <img src="https://swiperjs.com/demos/images/nature-1.jpg" />
      </div> </swiper-slide
    ><swiper-slide>
      <div class="swiper-zoom-container">
        <img src="https://swiperjs.com/demos/images/nature-2.jpg" />
      </div> </swiper-slide
    ><swiper-slide>
      <div class="swiper-zoom-container">
        <img src="https://swiperjs.com/demos/images/nature-3.jpg" />
      </div> </swiper-slide>
      
  </swiper>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/zoom';
import 'swiper/css/navigation';
import 'swiper/css/pagination';

import '../assets/cssBlog/style.scss';

// import required modules
import { Zoom, Navigation, Pagination } from 'swiper/modules';
    export default {
        name:'SwipersComponents',
        components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Zoom, Navigation, Pagination],
        
      };
      
    },
    }
</script>

<style lang="scss" scoped>
.swiper-container {
  /* Измените стили контейнера здесь */
  background-color: #f1f1f1;
  border: 1px solid #ddd;
}
.swiper-button-next::after{color: black;}
#app { height: 100% }
html,
body {
  position: relative;
  height: 100%;
}

body {
  background: #eee;
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  font-size: 14px;
  color: #000;
  margin: 0;
  padding: 0;
}

body {
  background: #000;
}
.swiper-button-next{
  color: #000;
}
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  overflow: hidden;
}
.swiper-button-prev::after{
  color: #000;
}


</style>