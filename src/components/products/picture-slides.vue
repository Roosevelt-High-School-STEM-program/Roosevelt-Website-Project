<template>
  <q-carousel
    :style="carouselSize"
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
      :name="1"
      :img-src="photos[0]"
      style="background-size: cover"
    >
      <div class="absolute-top custom-caption">
        <div :class="this.$q.screen.lt.sm ? 'text-h4' : 'text-h2'">
          <slot name="picture-name1" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide
      :name="2"
      :img-src="photos[1]"
      style="background-size: cover"
    >
      <div class="absolute-top custom-caption">
        <div :class="this.$q.screen.lt.sm ? 'text-h4' : 'text-h2'">
          <slot name="picture-name2" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide
      :name="3"
      :img-src="photos[2]"
      style="background-size: cover"
    >
      <div class="absolute-top custom-caption">
        <div :class="this.$q.screen.lt.sm ? 'text-h4' : 'text-h2'">
          <slot name="picture-name3" />
        </div>
      </div>
    </q-carousel-slide>
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
      slide: 1,
    };
  },
  computed: {
    carouselSize() {
      if (this.$q.screen.gt.sm && this.$q.screen.lt.lg) {
        return 'height: 450px;';
      }
      if (this.$q.screen.lt.sm || this.$q.screen.sm) {
        return 'height: 320px';
      }
      return 'height: 550px';
    },
  },
};
</script>

<style scoped>
  .custom-caption {
    text-align: center;
    padding: 12px;
    color: white;
    background-color: rgba(0, 0, 0, .3);
  }
</style>
