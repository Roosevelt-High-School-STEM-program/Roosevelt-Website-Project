<template>
  <div>
    <div class="row">
      <div class="col-md"></div>
      <div class="col-lg-5 col-md-12 col-xs-12 justify-center">
        <div class="col-12">
          <h1
            class="q-ml-lg q-my-none text-weight-bolder title"
            :style="resizableHeadersFont"
          >
            <slot name="product-title" />
          </h1>
          <div class="q-my-md q-mx-lg black-border" />
          <p :class="resizableMarginDescription" :style="resizableFont">
            <slot name="product-description" />
          </p>
        </div>

        <picture-slides
          v-show="$q.screen.sm || $q.screen.lt.lg"
          :class="resizableMarginCarousel"
          :photos="photos"
        >
<!--          <template v-slot:picture-name1><slot name="picture-name1" /></template>-->
<!--          <template v-slot:picture-name2><slot name="picture-name2" /></template>-->
<!--          <template v-slot:picture-name3><slot name="picture-name3" /></template>-->
        </picture-slides>
<!--        <h1-->
<!--          class="q-ml-lg q-mb-none q-mt-lg text-weight-bolder title"-->
<!--          :style="resizableHeadersFont"-->
<!--        >-->
<!--          Where to Find it-->
<!--        </h1>-->
<!--        <div class="q-mb-md q-mx-lg black-border" />-->
<!--        <div class="row q-ma-md">-->
<!--          <address-component-->
<!--            v-for="(location, index) in locations"-->
<!--            :key="index"-->
<!--            :class="resizableMarginAddresses" @on-submit="openLocation(index)"-->
<!--          >-->
<!--            <template v-slot:name>{{ locations[index].name }}</template>-->
<!--            <template v-slot:street>{{ locations[index].street }}</template>-->
<!--            <template v-slot:city>{{ locations[index].city }}</template>-->
<!--          </address-component>-->
<!--        </div>-->
      </div>
      <div class="col-md"/>
      <picture-slides
        v-show="!$q.screen.lt.lg"
        :class="$q.screen.lg ? 'col-lg-6':'col-lg-12'"
        :photos="photos"
      >
        <template v-slot:picture-name1><slot name="picture-name1" /></template>
        <template v-slot:picture-name2><slot name="picture-name2" /></template>
        <template v-slot:picture-name3><slot name="picture-name3" /></template>
      </picture-slides>
      <div class="col-md"></div>
    </div>
  </div>
</template>

<script>
// import AddressComponent from './address-component';
import PictureSlides from './picture-slides';

export default {
  name: 'product-component',
  components: {
    PictureSlides,
    // AddressComponent
  },
  props: {
    photos: {
      type: Array,
      default() {
        return [];
      },
    },
    locations: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  data() {
    return {
      slide: 1,
    };
  },
  methods: {
    openLocation(index) {
      window.open(`https://www.google.com//maps?q=${this.locations[index].name} ${this.locations[index].street}, ${this.locations[index].city}`);
    },
  },
  computed: {
    resizableFont() {
      return this.$q.screen.lt.sm ? 'font-size:17px;' : 'font-size:19px;';
    },
    resizableHeadersFont() {
      return this.$q.screen.lt.sm ? 'font-size: 45px;' : '';
    },
    resizableMarginDescription() {
      return this.$q.screen.sm || this.$q.screen.lt.sm ? 'q-mt-lg q-mx-xl anaheim' : 'q-mt-xl q-mx-xl anaheim';
    },
    resizableMarginCarousel() {
      if (this.$q.screen.gt.sm && this.$q.screen.lt.lg) {
        return 'col-sm-12 q-mt-lg q-mx-xl';
      }
      if (this.$q.screen.sm || this.$q.screen.lt.sm) {
        return 'col-sm-12 q-mt-lg';
      }
      return 'q-mt-xl';
    },
    // resizableMarginAddresses() {
    // return this.$q.screen.sm || this.$q.screen.lt.sm ?
    // 'col-md-6 col-sm-6 col-xs-11 q-mt-lg' : 'col-md-6 col-sm-6 col-xs-11 q-mb-sm';
    // },
  },
};
</script>

<style scoped>
  .title {
    font-family: Alegreya Sans SC;
    font-size:50px;
    letter-spacing: 2px
  }
</style>
