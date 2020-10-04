<template>
  <div>
    <about-us class="q-mt-md" id="about"/>
    <certification-banner class="q-mt-md" />
    <our-ohana />
  </div>
</template>

<script>
import AboutUs from '../components/aboutus/AboutUs';
import CertificationBanner from './CertificationBanner';
import OurOhana from '../components/aboutus/OurOhana';

export default {
  name: 'About',
  components: {
    AboutUs,
    CertificationBanner,
    OurOhana,
  },
};
</script>
