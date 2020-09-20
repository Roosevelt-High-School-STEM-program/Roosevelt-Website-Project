<template>
  <q-page>
    <regular-opening-screen id="opening-screen" />
    <about id="about"/>
    <products id="brands" />
    <regular-contact-us />
  </q-page>
</template>

<script>
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';
import RegularContactUs from '../components/contactus/RegularContactUs';
import Products from '../pages/Products';
import About from './About';

export default {
  name: 'Index',
  components: {
    About,
    RegularOpeningScreen,
    RegularContactUs,
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
      } else if (this.$q.screen.sm) {
        window.scroll({
          top: divPosition - 65,
          behavior: 'smooth',
        });
      } else if (this.$q.screen.lt.sm) {
        window.scroll({
          top: divPosition - 210,
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
