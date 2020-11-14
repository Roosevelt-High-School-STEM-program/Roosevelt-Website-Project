<template>
  <q-carousel
    :style="resizableCarousel"
    class="q-ml-lg q-mt-lg q-mr-lg order-second float-image"
    animated
    v-model="slide"
    transition-prev="slide-right"
    transition-next="slide-left"
    flat
    arrows
    navigation
    infinite
  >
    <q-carousel-slide
      v-for="(x, index) in photos"
      :key="index+fixIndex"
      :name="index+fixIndex"
      :img-src="x"
      style="background-size: cover"
    >
<!--      <div class="absolute-top custom-caption text-weight-bold">-->
<!--        <div :class="resizableHeader">-->
<!--          <slot name="picture-name1" />-->
<!--        </div>-->
<!--      </div>-->
    </q-carousel-slide>
<!--    <q-carousel-slide-->
<!--      :name="2"-->
<!--      :img-src="photos[1]"-->
<!--      style="background-size: cover"-->
<!--    >-->
<!--      <div class="absolute-top custom-caption">-->
<!--        <div :class="resizableHeader">-->
<!--          <slot name="picture-name2" />-->
<!--        </div>-->
<!--      </div>-->
<!--    </q-carousel-slide>-->
<!--    <q-carousel-slide-->
<!--      :name="3"-->
<!--      :img-src="photos[2]"-->
<!--      style="background-size: cover"-->
<!--    >-->
<!--      <div class="absolute-top custom-caption">-->
<!--        <div :class="resizableHeader">-->
<!--          <slot name="picture-name3" />-->
<!--        </div>-->
<!--      </div>-->
<!--    </q-carousel-slide>-->
  </q-carousel>
</template>

<script>
export default {
  name: 'picture-slides',
  props: {
    photos: {
      type: Array,
      default: null,
    },
  },
  data() {
    return {
      fixIndex: 1,
      slide: 1,
    };
  },
  computed: {
    resizableCarousel() {
      if (this.$q.screen.gt.sm && this.$q.screen.lt.lg) {
        return 'height: 450px;';
      }
      if (this.$q.screen.lt.sm || this.$q.screen.sm) {
        return '';
      }
      return 'height: 450px; width:740px';
    },
    resizableHeader() {
      return this.$q.screen.lt.sm ? 'text-h4' : 'text-h3';
    },
  },
};
</script>

<style scoped>
  /*.custom-caption {*/
  /*  text-align: center;*/
  /*  padding: 12px;*/
  /*  color: white;*/
  /*  background-color: rgba(0, 0, 0, .3);*/
  /*  font-family: Alegreya Sans SC, cursive;*/
  /*}*/
</style>
