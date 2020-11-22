<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header elevated class="text-black bg-white">
        <q-toolbar style="font-family: Alegreya Sans SC;">
          <div>
<!--            <q-img-->
<!--              style="height:50px; width:70px; cursor: pointer;"-->
<!--              src="../statics/icons/HonoluluBakingLogoBlackWhite.png"-->
<!--              @click="teleport('#opening-screen')"-->
<!--            />-->
<!--            TODO await opinions from the baking comp-->
            <q-img
              style="height:46px; width:227px; cursor: pointer;"
              src="../statics/icons/BlackWhiteContactLogo.png"
              @click="teleport('#opening-screen')"
            />
          </div>
          <div v-show="$q.screen.sm || $q.screen.gt.sm" style="width:100%">
            <q-btn
              style="letter-spacing: 3px;"
              size="14px"
              flat
              class="float q-pa-sm text-weight-bold"
              @click="delivery"
              label="ORDER ONLINE"
              name="ORDER ONLINE"
            />
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
        </q-toolbar>
        <q-list v-show="drawer">
          <q-item v-for="(name, index) in navigationNames" :key="name" v-ripple>
            <q-item-section
              class="text-weight-bold"
              style="letter-spacing: 3px; font-size: 14px"
              @click="name != 'ORDER ONLINE' ? teleport('#' + navigationId[index]) : delivery()"
            >
              {{ name }}
            </q-item-section>
          </q-item>
        </q-list>
      </q-header>

      <q-page-container>
        <router-view />
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>

export default {
  name: 'Layout',
  data() {
    return {
      drawer: false,
      navigationNames: [
        'OUR STORY',
        'OUR BRANDS',
        'ORDER ONLINE',
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
      // if ($q.screen.sm) {
      //
    },
    delivery() {
      window.open('https://www.grubhub.com/restaurant/honolulu-baking-company-523-ahui-st-honolulu/2048001');
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
</style>
