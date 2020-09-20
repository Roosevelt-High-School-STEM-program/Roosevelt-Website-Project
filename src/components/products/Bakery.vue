<template>
  <div style="min-height: 800px">
    <div class="row">
      <div class="col-md"></div>
      <div class="col-lg-5 col-md-12 col-xs-12">
        <h1
          class="q-ml-lg q-my-none text-weight-bolder title"
          :style="resizableHeadersFont"
        >
          Bakery
        </h1>
        <div class="q-my-md q-mx-lg black-border" />
        <p :class="resizableMarginDescription" :style="resizableFont">
          It is a long established fact that a reader will be distracted by
          the readable content of a page when looking at its layout. The point of using Lorem I
          psum is that it has a more-or-less normal distribution of letters, as opposed to using
        </p>
        <picture-slides
          v-show="$q.screen.sm || $q.screen.lt.lg"
          :class="resizableMarginCarousel"
          :photos="photos"
        >
          <template v-slot:picture-name1>Lemon Scone</template>
          <template v-slot:picture-name2>Blueberry Scone</template>
          <template v-slot:picture-name3>Blueberry Scone</template>
        </picture-slides>
        <h1
          class="q-ml-lg q-mb-none q-mt-lg text-weight-bolder title"
          :style="resizableHeadersFont"
        >
          Where to Find it
        </h1>
        <div class="q-mb-md q-mx-lg black-border" />
        <div class="row q-ma-md">
          <address-component
            v-for="(location, index) in locations"
            :key="index"
            :class="resizableMarginAddresses" @on-submit="openLocation(x)"
          >
            <template v-slot:name>{{ locations[index].name }}</template>
            <template v-slot:street>{{ locations[index].street }}</template>
            <template v-slot:city>{{ locations[index].city }}</template>
          </address-component>
        </div>
      </div>
      <div class="col-md"/>
<!--      // col-md-6  col-sm order-second-->
      <picture-slides
        v-show="!($q.screen.lt.lg)"
        class="col-lg-6"
        :photos="photos"
      >
        <template v-slot:picture-name1>Lemon Scone</template>
        <template v-slot:picture-name2>Blueberry Scone</template>
        <template v-slot:picture-name3>Blueberry Scone</template>
      </picture-slides>
      <div class="col-md"></div>
    </div>
  </div>
</template>

<script>
import AddressComponent from './address-component';
import PictureSlides from './picture-slides';

export default {
  name: 'Bakery',
  components: { PictureSlides, AddressComponent },
  data() {
    return {
      slide: 1,
      slotNames: ['place', 'address', 'city'],
      photos: [
        '../../statics/scones.jpeg',
        '../../statics/rotating-photos/blueBerryPastries.jpeg',
        '../../statics/rotating-photos/orangePastries.png',
      ],
      locations: [
        {
          name: 'Walmart',
          street: '700 Ke’eaumoku St',
          city: 'Honolulu, HI 96814',
        },
        {
          name: 'Cultural Pa',
          street: '100 N Beretania St',
          city: 'Honolulu, HI 96817',
        },
        {
          name: 'Cultural Plaza',
          street: '100 N Beretania St',
          city: 'Honolulu, HI 96817',
        },
        {
          name: 'Cultural Plaza',
          street: '100 N Beretania St',
          city: 'Honolulu, HI 96817',
        },
      ],
    };
  },
  methods: {
    openLocation(index) {
      window.open(`https://www.google.com//maps?q=${this.locations[index].name} ${this.locations[index].street}, ${this.locations[index].city}`);
    },
  },
  computed: {
    resizableFont() {
      if (this.$q.screen.lt.sm) {
        return 'font-size:17px;';
      }
      return 'font-size:19px;';
    },
    resizableHeadersFont() {
      if (this.$q.screen.lt.sm) {
        return 'font-size: 45px;';
      }
      return '';
    },
    resizableMarginDescription() {
      if (this.$q.screen.sm || this.$q.screen.lt.sm) {
        return 'q-mt-lg q-mx-xl anaheim';
      }
      return 'q-mt-xl q-mx-xl anaheim';
    },
    resizableMarginCarousel() {
      if (this.$q.screen.gt.sm && this.$q.screen.lt.lg) {
        return 'col-sm-12 q-mt-lg q-mx-xl';
      }
      if (this.$q.screen.sm || this.$q.screen.lt.sm) {
        return 'col-sm-12 q-mt-lg';
      }
      return 'col-sm-12 q-mt-xl';
    },
    resizableMarginAddresses() {
      if (this.$q.screen.sm || this.$q.screen.lt.sm) {
        return 'col-md-6 col-sm-6 col-xs-11 q-mb-sm';
      }
      return 'col-md-6 col-sm-6 col-xs-11 q-mt-lg';
    },
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
