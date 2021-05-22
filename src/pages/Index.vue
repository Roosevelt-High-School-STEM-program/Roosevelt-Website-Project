<template>
  <q-page>
    <navigation-bar id="opening-screen" />
    <about id="about"/>
    <products class="q-mt-lg" id="brands" />
    <contact-us />
  </q-page>
</template>

<script>
import NavigationBar from '../components/navigationBar';
import ContactUs from '../components/contactus/ContactUs';
import Products from '../pages/Products';
import About from './About';

export default {
  name: 'Index',
  components: {
    About,
    NavigationBar,
    ContactUs,
    Products,
  },
  methods: {
    scrollTo(select) {
      const divPosition = document.querySelector(select).getBoundingClientRect().top
          + window.scrollY;
      if (this.$q.screen.lt.sm) {
        window.scroll({
          top: divPosition - 160,
          behavior: 'smooth',
        });
      } else {
        window.scroll({
          top: divPosition,
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
