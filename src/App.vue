<template>
  <div class="appwrapper">

    <div class="container mx-auto">
      <carousel>
        <slide key="1">
          <Tabs />
        </slide>
        <slide key="2">
          <Gallery />
        </slide>

        <template #addons>

          <pagination />
        </template>
      </carousel>

    </div>
  </div>
</template>

<script>

import 'vue3-carousel/dist/carousel.css'
import './assets/main.css'


import { Carousel, Slide, Pagination } from 'vue3-carousel'

import Tabs from "./components/Tabs.vue";
import Gallery from "./components/Gallery.vue";

export default {
  name: 'App',
  created() {
    document.title = "BinhNS Test Result Vue ";
  },
  components: {
    Carousel,
    Slide,
    Pagination,
    Tabs,
    Gallery
  }
}
</script>

<style scoped>
.appwrapper {
  padding-top: 108px;
}



@media(max-width: 767px) {
  .appwrapper {
    padding-top: 0;
  }
}
</style>