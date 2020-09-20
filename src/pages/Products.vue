<template>
  <div class="row justify-center">
    <div class="col-md-4 col-sm-8 col-xs-12 q-mb-lg">
      <q-img src="../../src/statics/Products2.png"></q-img>
    </div>
    <bakery class="col-md-12" />
    <!-- covert to a component -->
    <div class="q-mx-xl q-my-xl col black-border" />
    <bakery class="col-md-12 q-mb-xl" />
<!--    <hand-cut-produce class="col-md-12 col-md-12 q-mb-xl" />-->
  </div>
</template>

<script>
// import HandCutProduce from '../components/products/HandCutProduce';
import Bakery from '../components/products/Bakery';

export default {
  name: 'Products',
  components: {
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
