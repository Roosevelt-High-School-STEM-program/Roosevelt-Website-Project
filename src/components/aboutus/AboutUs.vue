<template>
  <div
    class="row justify-center items-center bg-white"
    style="min-height:520px"
  >
    <div class="col-md-1 col-xs-8 q-mt-none" />
    <div class="col-md-4 col-xs-11">
      <h1
        class="q-my-none text-weight-bold text-center"
        style="font-size: 45px; letter-spacing: 2px;"
      >
        Our Story
      </h1>
      <p
        :class="$q.screen.sm || $q.screen.lt.sm ? 'anaheim' : 'anaheim q-mt-sm'"
        :style="$q.screen.lt.sm ? 'font-size:17px;' : 'font-size:20px;'"
      >
        In 1997, we began our journey as the primary food supplier for local
        Starbucks stores in Hawaii. Today, we offer a wide variety of sweet
        and savory treats in a broad range of grocery, club, and convenience stores in Hawaii.
        You can even buy our famous Original Oatcake and other goodies directly
        from our bakery in Kaka'ako.
        <br>
        <br>
        We believe food connects us with our family, friends, and community.
        Food is good for the soul!
      </p>
    </div>
    <div class="col-md-2" />
    <div
      :class="$q.screen.sm || $q.screen.lt.sm ?
        'row justify-center col-xs-8 col-sm-12 order-first q-mt-lg' : 'row col-md-3 justify-center'"
    >
      <q-img
        class="float-image"
        :style="$q.screen.sm || $q.screen.lt.sm ? 'max-width:280px' : 'max-width:320px'"
        src="../../statics/food-pictures/oatCakeTopDown.png"
      />
    </div>
    <div class="col-md-2"/>
  </div>
</template>

<script>

export default {
  name: 'AboutUs',
};
</script>

<style scoped>
  h1 {
    font-family: Alegreya Sans SC, cursive;
  }
</style>
