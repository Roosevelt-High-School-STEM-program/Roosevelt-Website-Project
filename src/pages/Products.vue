<template>
  <div class="row justify-center">
    <q-img
      class="col-md-3 col-sm-5 col-xs-8 q-mb-lg"
      src="../../src/statics/ourBrand.png"
    />
    <honolulu-baking-company class="col-md-12" />
    <div class="q-mx-xl q-my-xl col black-border" />
    <honolulu-fresh-cut class="col-md-12" />
    <div class="q-mx-xl q-my-xl col black-border" />
    <kakaako-eats class="col-md-12 q-mb-xl" />
  </div>
</template>

<script>
import HonoluluBakingCompany from '../components/products/HonoluluBakingCompany';
import HonoluluFreshCut from '../components/products/HonoluluFreshCut';
import KakaakoEats from '../components/products/KakaakoEats';

export default {
  name: 'Products',
  components: {
    HonoluluBakingCompany,
    KakaakoEats,
    HonoluluFreshCut,
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
