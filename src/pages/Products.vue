<template>
  <div class="row justify-center">
    <q-img
      class="col-md-3 col-sm-5 col-xs-8 q-mb-lg"
      src="../../src/statics/ourBrand.png"
    />
    <bakery class="col-md-12" />
    <!-- covert to a component -->
    <div class="q-mx-xl q-my-xl col black-border" />
    <hand-cut-produce class="col-md-12 q-mb-xl" />

  </div>
</template>

<script>
// import HandCutProduce from '../components/products/HandCutProduce';
import Bakery from '../components/products/Bakery';
import HandCutProduce from '../components/products/HandCutProduce';

export default {
  name: 'Products',
  components: {
    HandCutProduce,
    Bakery,
    // HandCutProduce,
  },
};
</script>

<style scoped>
  h1 {
    font-size: 106px;
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
  }
</style>
