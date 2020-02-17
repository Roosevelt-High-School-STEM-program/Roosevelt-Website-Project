<template>
  <q-page>
    <regular-opening-screen />
    <regular-about-us />
    <regular-workers-screen />
    <regular-contact-us id="gay"/>
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularAboutUs from '../components/aboutus/RegularAboutUs';
import RegularContactUs from '../components/contactus/RegularContactUs';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';

export default {
  name: 'PageIndex',
  components: {
    RegularContactUs, RegularWorkersScreen, RegularOpeningScreen, RegularAboutUs,
  },
};
</script>
