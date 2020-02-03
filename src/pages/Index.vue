<template>
  <q-page>
    <regular-opening-screen></regular-opening-screen>
    <regular-about-us></regular-about-us>
    <regular-workers-screen></regular-workers-screen>
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularAboutUs from '../components/aboutus/RegularAboutUs';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';

export default {
  name: 'PageIndex',
  components: { RegularWorkersScreen, RegularOpeningScreen, RegularAboutUs },
};
</script>
