<template>
  <div>
    <q-layout view="hHh lpR fFf">
      <q-header
        class="text-white transparent"
        height-hint="98"
      >
        <q-toolbar
          class="text-dark"
          style="font-family: Satisfy, cursive; height: 20px;"
        >
          <q-toolbar-title>
            Honolulu Baking Company
          </q-toolbar-title>
<!--          <q-tabs-->
<!--            alight-left-->
<!--            class="text-dark"-->
<!--            style="font-family: Satisfy, cursive;"-->

<!--          >-->
            <q-btn @click="teleport('#about-us')" name="hello">ABOUT US</q-btn>
          <q-btn @click="teleport('#ohana')" name="hello">OHANA</q-btn>
            <q-btn @click="teleport('#contact-us')" name="hello">CONTACT</q-btn>
<!--            <q-route-tab name="About Us" onclick="teleport()">-->
<!--              <div class="text-weight-bold">ABOUT US</div>-->
<!--            </q-route-tab>-->
<!--            <q-route-tab to="/page2" name="Contacts">-->
<!--              <div class="text-weight-bold">CONTACTS</div>-->
<!--            </q-route-tab>-->
<!--            <q-route-tab to="/page3" name="Clients">-->
<!--              <div class="text-weight-bold">CLIENTS</div>-->
<!--            </q-route-tab>-->
<!--          </q-tabs>-->
        </q-toolbar>

      </q-header>
      <q-page-container>
        <regular-opening-screen />
        <regular-about-us id="about-us" />
        <regular-workers-screen id="ohana"/>
        <regular-contact-us id="contact-us" />
      </q-page-container>
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
