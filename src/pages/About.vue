<template>
  <div>
    <about-us class="q-mt-md" id="about"/>
    <certification-banner class="q-mt-md" />
    <workers-screen class="$q.screen.gt.sm ? '' : 'q-mb-xl'" />
  </div>
</template>

<script>
import AboutUs from '../components/aboutus/AboutUs';
import CertificationBanner from './CertificationBanner';
import WorkersScreen from '../components/aboutus/WorkersScreen';

export default {
  name: 'About',
  components: {
    AboutUs,
    CertificationBanner,
    WorkersScreen,
  },
};
</script>

<style scoped>

</style>
