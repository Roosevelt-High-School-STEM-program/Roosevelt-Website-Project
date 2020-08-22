<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header
        class="text-white transparent"
        height-hint="98"
      >
        <q-toolbar
          class="text-dark"
          style="font-family: Alegreya Sans SC; height: 20px;"
        >
          <div class="col-md-6"></div>
          <div class="col-md-6 row justify-end text-website-page-cutter-red">
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#about')"
              name="hello"
            >
              ABOUT
            </q-btn>
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#ohana')"
              name="hello"
            >
              OHANA
            </q-btn>
            <q-btn
              style="letter-spacing: 3px; font-size: 15px"
              flat
              class="col-md-2 q-pa-sm q-ml-md text-weight-bold"
              @click="teleport('#contact-us')"
              name="hello"
            >
              CONTACT
            </q-btn>
          </div>
        </q-toolbar>

      </q-header>
        <regular-opening-screen />
        <regular-about id="about"/>
        <regular-workers-screen id="ohana"/>
        <regular-contact-us id="contact-us" />
    </q-layout>
  </div>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';
import RegularContactUs from '../components/contactus/RegularContactUs';
import RegularAbout from '../components/aboutus/RegularAbout';

export default {
  name: 'Layout',
  components: {
    RegularAbout,
    RegularContactUs,
    RegularWorkersScreen,
    RegularOpeningScreen,
  },
  data() {
    return {
    };
  },
  methods: {
    teleport(select) {
      // eslint-disable-next-line no-restricted-globals
      document.querySelector(select).scrollIntoView({ behavior: 'smooth' });
    },
  },
};
</script>

<style scoped>
  template {
    scroll-behavior: smooth;
  }

</style>
