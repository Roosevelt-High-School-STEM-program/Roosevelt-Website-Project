<template>
  <div col="row">
    <div class="col-md-12 ">
      <h1 class="q-my-lg text-weight-medium">
        products
      </h1>
    </div>
    <bakery class="col-md-12" />
    <hand-cut-produce class="col-md-12" />
  </div>
</template>

<script>
import HandCutProduce from '../components/products/HandCutProduce';
import Bakery from '../components/products/Bakery';

export default {
  name: 'Products',
  components: { Bakery, HandCutProduce },
};
</script>

<style scoped>
  h1 {
    font-size: 106px;
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
  }

</style>
