<template>
  <div class="row justify-center float-navigation-bar">
    <div class="col-md-12 col-xs-12 row justify-center">
      <q-img
        :style="responsiveLogo"
        src="../statics/icons/hbclogo.png"
      />
    </div>
    <div class="col-md-8"/>
    <div class="col-md-4" v-show="$q.screen.sm || $q.screen.gt.sm" style="width:100%">
      <!-- WIP TODO add online ordering-->
      <!--      <q-btn-->
<!--        style="letter-spacing: 3px;"-->
<!--        size="14px"-->
<!--        flat-->
<!--        class="float q-pa-sm text-weight-bold"-->
<!--        @click="delivery"-->
<!--        label="ORDER ONLINE"-->
<!--        name="ORDER ONLINE"-->
<!--      />-->
      <q-btn
        style="letter-spacing: 3px;"
        size="14px"
        flat
        class="float q-pa-sm text-weight-bold"
        @click="teleport('#brands')"
        label="OUR BRANDS"
        name="OUR BRANDS"
      />
      <q-btn
        style="letter-spacing: 3px;"
        size="14px"
        flat
        class="float q-pa-sm text-weight-bold"
        @click="teleport('#about')"
        label="OUR STORY"
        name="OUR STORY"
      />
    </div>
    <div v-show="$q.screen.lt.sm" style="width:100%">
      <q-btn dense flat round icon="menu" @click="drawer = !drawer" class="float" />
    </div>
    <q-list class="col-12" v-show="drawer && $q.screen.lt.sm">
      <q-item v-for="(name, index) in navigationNames" :key="name" clickable v-ripple>
        <q-item-section
          class="text-weight-bold text-center"
          style="letter-spacing: 3px; font-size: 14px"
          @click="teleport('#' + navigationId[index])"
        >
          {{ name }}
        </q-item-section>
      </q-item>
    </q-list>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      navigationNames: [
        'OUR STORY',
        'OUR BRANDS',
      ],
      navigationId: [
        'about',
        'brands',
      ],
    };
  },
  methods: {
    teleport(select) {
      this.drawer = false;
      this.$root.$emit('on-submit', select);
    },
    // delivery() {
    //   window.open('https://www.grubhub.com/restaurant/honolulu-baking-company-523-ahui-st-honolulu/2048001');
    // },
  },
  computed: {
    responsiveLogo() {
      return this.$q.screen.lt.sm ? 'height:130px; width: 190px;' : 'height:170px; width: 240px;';
    },
  },
};
</script>

<style scoped>
  template {
    scroll-behavior: smooth;
  }
  .float {
    float: right !important;
  }
  .float-navigation-bar {
    box-shadow: 5px 0px 10px 3px grey;
  }
</style>
