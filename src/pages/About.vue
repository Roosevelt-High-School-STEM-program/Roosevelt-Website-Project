<template>
  <div>
    <regular-about class="q-mt-md" id="about"/>
    <certification-banner class="q-mt-md" />
    <regular-workers-screen />
  </div>
</template>

<script>
import RegularAbout from '../components/aboutus/RegularAbout';
import CertificationBanner from './CertificationBanner';
import RegularWorkersScreen from '../components/aboutus/RegularWorkersScreen';

export default {
  name: 'About',
  components: {
    RegularAbout,
    CertificationBanner,
    RegularWorkersScreen,
  },
};
</script>

<style scoped>

</style>
