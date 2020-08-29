<template>
  <q-page>
    <regular-opening-screen />
    <regular-about id="about"/>
    <regular-workers-screen id="ohana"/>
    <products id="products" />
    <regular-contact-us id="contact-us" />
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularAbout from '../components/aboutus/RegularAbout';
import RegularContactUs from '../components/contactus/RegularContactUs';
import RegularWorkersScreen from '../components/workersscreen/RegularWorkersScreen';
import Products from '../pages/Products';

export default {
  name: 'Index',
  components: {
    RegularOpeningScreen,
    RegularAbout,
    RegularContactUs,
    RegularWorkersScreen,
    Products,
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
