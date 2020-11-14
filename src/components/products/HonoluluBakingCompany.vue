<template>
  <product-component
    :locations="locations"
    :photos="photos"
  >
    <template v-slot:product-title>Honolulu Baking Company</template>
    <template v-slot:product-description>
      Wholesale sweet and savory baked goods - cookies, scones, muffins, our very own
      Original Oatcake, pizzas, and breakfast sandwiches. If you own a small cafe and
      are looking for food to sell, give us a call. Our cafe program is an all-inclusive
      option. We work with you to prepare the menu and will deliver to your cafe!
    </template>
    <template v-slot:picture-name1>Lemon Scone</template>
    <template v-slot:picture-name2>Blueberry Scone</template>
    <template v-slot:picture-name3>wasd</template>
  </product-component>
</template>

<script>
import ProductComponent from './product-component';

export default {
  name: 'HonoluluBakingCompany',
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
