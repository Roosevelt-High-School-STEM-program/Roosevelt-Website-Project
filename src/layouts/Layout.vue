<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header
        class="text-white transparent"
        height-hint="98"
      >
        <q-toolbar
          class="text-dark"
          style="font-family: 'Alegreya Sans SC', sans-serif; height: 20px;"
        >
          <div class="col-12 float-right">
            <q-btn
              flat
              class="q-pa-sm float-right q-ml-md"
              @click="teleport('#about-us')"
              name="hello"
            >
              ABOUT US
            </q-btn>
            <q-btn
              flat
              class="float-right q-pa-sm q-ml-md"
              @click="teleport('#ohana')"
              name="hello"
            >
              OHANA
            </q-btn>
            <q-btn
              flat
              class="float-right q-pa-sm q-ml-md"
              @click="teleport('#contact-us')"
              name="hello"
            >
              CONTACT
            </q-btn>
          </div>
        </q-toolbar>

      </q-header>
        <regular-opening-screen />
        <regular-about-us id="about-us" />
        <regular-workers-screen id="ohana"/>
        <regular-contact-us id="contact-us" />
    </q-layout>
  </div>
</template>

<script>
import RegularAboutUs from '../components/aboutus/RegularAboutUs';
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';
import RegularContactUs from '../components/contactus/RegularContactUs';

export default {
  name: 'Layout',
  components: {
    RegularContactUs, RegularWorkersScreen, RegularOpeningScreen, RegularAboutUs,
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
