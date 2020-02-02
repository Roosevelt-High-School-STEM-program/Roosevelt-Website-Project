<template>
  <q-page>
    <regular-opening-screen></regular-opening-screen>
    <regular-about-us></regular-about-us>
    <regular-opening-screen></regular-opening-screen>
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularAboutUs from '../components/aboutus/RegularAboutUs';

export default {
  name: 'PageIndex',
  components: { RegularOpeningScreen, RegularAboutUs },
};
</script>
