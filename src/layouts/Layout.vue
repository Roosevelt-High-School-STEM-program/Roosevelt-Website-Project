<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header
        class="text-white transparent"
      >
        <q-toolbar
          style="font-family: Alegreya Sans SC; height: 20px;"
        >
          <div class="col-md-6"></div>
          <div class="col-md-6 row justify-end text-website-page-cutter-red">
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#about')"
              name="about"
            >
              about
            </q-btn>
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#ohana')"
              name="ohana"
            >
              ohana
            </q-btn>
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#products')"
              name="products"
            >
              products
            </q-btn>
<!--            <q-btn-->
<!--              style="letter-spacing: 3px; font-size: 15px"-->
<!--              flat-->
<!--              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"-->
<!--              @click="teleport('#bakery')"-->
<!--              name="hello"-->
<!--            >-->
<!--              bakery-->
<!--            </q-btn>-->
<!--            <q-btn-->
<!--              style="letter-spacing: 3px; font-size: 15px"-->
<!--              flat-->
<!--              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"-->
<!--              @click="teleport('#produce')"-->
<!--              name="hello"-->
<!--            >-->
<!--              produce-->
<!--            </q-btn>-->
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#contact-us')"
              name="contact"
            >
              contact
            </q-btn>
          </div>
        </q-toolbar>
      </q-header>
      <q-page-container style="padding: 0 0 0 0">
        <router-view />
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>

export default {
  name: 'Layout',
  methods: {
    teleport(select) {
      this.$root.$emit('on-submit', select);
    },
  },
};
</script>

<style scoped>
  template {
    scroll-behavior: smooth;
  }

</style>
