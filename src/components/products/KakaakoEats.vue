<template>
  <product-component
    :locations="locations"
    :photos="photos"
  >
    <template v-slot:product-title>Kaka'ako Eats <sup>TM</sup></template>
    <template v-slot:product-description>
      Complete meals meant to be shared with family and friends! We do all the cooking!
      All you do is heat and serve! See our menu (hyperlink?) here and give us a call.
      We take suggestions too!
    </template>
    <template v-slot:picture-name1>Lemon Scone</template>
    <template v-slot:picture-name2>Blueberry Scone</template>
    <template v-slot:picture-name3>wasd</template>
  </product-component>
</template>

<script>
import ProductComponent from './product-component';

export default {
  name: 'KakaakoEats',
  components: { ProductComponent },
  data() {
    return {
      photos: [
        '../../statics/rotating-photos/scones.jpg',
        '../../statics/rotating-photos/cake.jpg',
        '../../statics/rotating-photos/upsideDownCake.png',
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
};
</script>

<style scoped>

</style>
