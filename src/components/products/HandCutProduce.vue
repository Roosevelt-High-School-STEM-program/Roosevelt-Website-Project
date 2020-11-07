<template>
  <product-component
    :locations="locations"
    :photos="photos"
  >
    <template v-slot:product-title>Hand-cut products</template>
    <template v-slot:product-description>
      It is a long established fact that a reader will be distracted by
      the readable content of a page when looking at its layout. The point of using Lorem I
      psum is that it has a more-or-less normal distribution of letters, as opposed to using
    </template>
    <template v-slot:picture-name1>Lemon Scone</template>
    <template v-slot:picture-name2>Blueberry Scone</template>
    <template v-slot:picture-name3>wasd</template>
  </product-component>
</template>

<script>
import ProductComponent from './product-component';

export default {
  name: 'HandCutProduce',
  components: { ProductComponent },
  data() {
    return {
      photos: [
        '../../statics/rotating-photos/salad1.png',
        '../../statics/rotating-photos/salad2.jpg',
        '../../statics/rotating-photos/salad3.png',
      ],
      locations: [
        {
          name: 'Walmart',
          street: '700 Ke’eaumoku St',
          city: 'Honolulu, HI 96814',
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
