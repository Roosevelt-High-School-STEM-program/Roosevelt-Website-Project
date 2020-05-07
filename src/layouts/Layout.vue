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
          <div class="col-md-6 row justify-end text-website-light-brown">
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
        <regular-workers-screen-test id="ohana"/>
        <regular-contact-us id="contact-us" />
        <simple-test/>
    </q-layout>
  </div>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularWorkersScreenTest from '../components/workersscreen/RegularWorkerScreenTest';
import RegularContactUs from '../components/contactus/RegularContactUs';
import RegularAbout from '../components/aboutus/RegularAbout';
import SimpleTest from '../components/workersscreen/simpletest';

export default {
  name: 'Layout',
  components: {
    SimpleTest,
    RegularAbout,
    RegularContactUs,
    RegularWorkersScreenTest,
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
