<template>
  <product-component
    :locations="locations"
    :photos="photos"
  >
    <template v-slot:product-title>Honolulu Fresh Cut<sup>TM</sup></template>
    <template v-slot:product-description>
      Fresh prepared salads, fruits, and vegetables sold in local retail,
      club, and convenience stores. We hand cut our produce which reduces the amount
      of water left in the bowl so you get only the best fruits and veggies in our products.
    </template>
    <template v-slot:picture-name1>Lemon Scone</template>
    <template v-slot:picture-name2>Blueberry Scone</template>
    <template v-slot:picture-name3>wasd</template>
  </product-component>
</template>

<script>
import ProductComponent from './product-component.';

export default {
  name: 'HonoululuFreshCut',
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
