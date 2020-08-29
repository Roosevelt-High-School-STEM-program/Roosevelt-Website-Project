<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header elevated class="text-black bg-white">
        <q-toolbar style="font-family: Alegreya Sans SC;">
          <div>
            <q-img

              style="height:50px; width:70px; cursor: pointer;"
              src="../statics/icons/HonoluluBakingLogoBlackWhite.png"
              @click="teleport('#opening-screen')"
            />
          </div>
          <div style="width:100%">
            <q-btn
              style="letter-spacing: 3px;"
              size="14px"
              flat
              class="floatEm q-pa-sm text-weight-bold"
              @click="teleport('#contact-us')"
              name="contact"
            >
              contact
            </q-btn>
            <q-btn
              style="letter-spacing: 3px;"
              size="14px"
              flat
              class="floatEm q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#ohana')"
              name="ohana"
            >
              ohana
            </q-btn>
            <q-btn
              style="letter-spacing: 3px;"
              size="14px"
              flat
              class="floatEm q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#products')"
              name="products"
            >
              products
            </q-btn>
            <q-btn
              style="letter-spacing: 3px;"
              size="14px"
              flat
              class="floatEm q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#about')"
              name="about"
            >
              about
            </q-btn>
          </div>
        </q-toolbar>
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
  .floatEm {
    float: right !important;
  }
</style>
