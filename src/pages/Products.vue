<template>
  <div col="row">
    <div class="col-md-12">
      <h1 class="text-weight-medium text-center user-select: none;">
        products
      </h1>
    </div>
    <bakery class="col-md-12" />
    <div class="q-mx-xl q-my-xl" style="border-bottom:1px black solid;" />
    <bakery class="col-md-12 q-mb-xl" />

<!--    <hand-cut-produce class="col-md-12" />-->
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
