<template>
  <div style="height: 800px">
    <div class="row">
      <div class="col"></div>
      <div class="col-md-5">
        <h1
          class="q-ml-lg q-my-none text-weight-bolder title"
        >
          Bakery
        </h1>
        <div class="q-my-md q-mx-lg" style="border-bottom:1px black solid;" />
        <p class="q-mt-xl q-mx-xl" style="font-size:19px; font-family: 'Anaheim'">
          It is a long established fact that a reader will be distracted by
          the readable content of a page when looking at its layout. The point of using Lorem I
          psum is that it has a more-or-less normal distribution of letters, as opposed to using
          'Content here, content here', making it look like r
          eadable English. Many desktop publishing packages and web pa
          ge editors now use Lorem Ipsum as their default model text,
        </p>
        <h1
          class="q-ml-lg q-mb-none q-mt-xl text-weight-bolder title"
        >
          Where to Find it
        </h1>
        <div class="q-my-md q-mx-lg" style="border-bottom:1px black solid;" />

        <div class="row q-ma-md">
          <div class="col-md-6 q-mt-lg">
            <address-component>
              <template v-slot:place>Walmart</template>
              <template v-slot:address>1232 Nehoa Street</template>
              <template v-slot:city>Honolulu, Hi, 96822</template>
            </address-component>
          </div>
          <div class="col-md-6 q-mt-lg">
            <address-component>
              <template v-slot:place>Walmart</template>
              <template v-slot:address>1232 Nehoa Street</template>
              <template v-slot:city>Honolulu, Hi, 96822</template>
            </address-component>
          </div>
          <div class="col-md-6 q-mt-lg">
            <address-component>
              <template v-slot:place>Walmart</template>
              <template v-slot:address>1232 Nehoa Street</template>
              <template v-slot:city>Honolulu, Hi, 96822</template>
            </address-component>
          </div>
          <div class="col-md-6 q-mt-lg">
            <address-component>
              <template v-slot:place>Walmart</template>
              <template v-slot:address>1232 Nehoa Street</template>
              <template v-slot:city>Honolulu, Hi, 96822</template>
            </address-component>
          </div>
        </div>
      </div>
      <div class="col"/>
      <q-carousel
        style="height:550px"
        class="q-ml-lg q-mt-lg q-mr-lg col-md-6 float-image"
        animated
        v-model="slide"
        transition-prev="slide-right"
        transition-next="slide-left"
        flat
        arrows
        navigation
        infinite
      >
        <q-carousel-slide
          :name="1"
          img-src="../../statics/scones.jpeg" style="background-size: cover"
        >
          <div class="absolute-top custom-caption">
            <div class="text-h2">Lemon Scone</div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide
          :name="2"
          img-src="../../statics/rotating-photos/blueBerryPastries.jpeg"
          style="background-size: cover"
        >
          <div class="absolute-top custom-caption">
            <div class="text-h2">Blueberry Scone</div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide
          :name="3"
          img-src="../../statics/rotating-photos/orangePastries.png"
          style="background-size: cover"
        >
          <div class="absolute-top custom-caption">
            <div class="text-h2">Blueberry Scone</div>
          </div>
        </q-carousel-slide>
      </q-carousel>
      <div class="col-md"></div>
    </div>
  </div>
</template>

<script>
import AddressComponent from './address-component';

export default {
  name: 'Bakery',
  components: { AddressComponent },
  data() {
    return {
      slide: 1,
    };
  },
};
</script>

<style scoped>
  .title {
    font-family: Alegreya Sans SC;
    font-size:50px;
    letter-spacing: 2px
  }
  .custom-caption {
    text-align: center;
    padding: 12px;
    color: white;
    background-color: rgba(0, 0, 0, .3);
  }

</style>
