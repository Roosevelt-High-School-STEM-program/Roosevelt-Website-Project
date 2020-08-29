<template>
  <q-page>
    <regular-opening-screen id="opening-screen" />
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
      // length of the var too long
      const divPosition = document.querySelector(select).getBoundingClientRect().top
          + window.scrollY;
      if (divPosition < 0) {
        window.scroll({
          top: divPosition,
          behavior: 'smooth',
        });
      } else {
        window.scroll({
          top: divPosition - 52,
          behavior: 'smooth',
        });
      }
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
