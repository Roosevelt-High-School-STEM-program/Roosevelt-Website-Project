<template>
  <q-page>
    <regular-opening-screen />
    <regular-about id="about"/>
<!--    <regular-three-client-page />-->
    <regular-workers-screen id="ohana"/>
    <regular-contact-us id="contact-us" />
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
// import RegularThreeClientPage from '../components/threeclientpage/RegularThreeClientPage';
import RegularAbout from '../components/aboutus/RegularAbout';
import RegularContactUs from '../components/contactus/RegularContactUs';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';

export default {
  name: 'Index',
  components: {
    RegularOpeningScreen,
    // RegularThreeClientPage,
    RegularAbout,
    RegularContactUs,
    RegularWorkersScreen,
  },
  methods: {
    scrollTo(select) {
      document.querySelector(select).scrollIntoView({ behavior: 'smooth' });
    },
  },
  created() {
    this.$root.$on('on-submit', this.scrollTo);
  },
  beforeDestroy() {
    this.$root.$off('on-submit', this.scrollTo);
  },
};
</script>

<style scoped>

</style>
