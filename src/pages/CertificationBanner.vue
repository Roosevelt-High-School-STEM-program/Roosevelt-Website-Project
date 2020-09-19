<template>
  <div>
    <regular-certification-banner v-show="!($q.screen.sm || $q.screen.lt.sm)" />
    <mobile-certification-banner class="q-mt-md" v-show="$q.screen.sm || $q.screen.lt.sm" />
  </div>
</template>

<script>
import MobileCertificationBanner from '../components/aboutus/MobileCertficationBanner';
import RegularCertificationBanner from '../components/aboutus/RegularCertificationBanner';

export default {
  name: 'CertificationBanner',
  components: { MobileCertificationBanner, RegularCertificationBanner },
};
</script>

<style scoped>

</style>
