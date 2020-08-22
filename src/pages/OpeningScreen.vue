<template>
  <regular-opening-screen v-if="$q.screen.gt.sm" />
  <mobile-opening-screen v-else />
</template>

<script>
import MobileOpeningScreen from '../components/openingscreen/MobileOpeningScreen';
import RegularOpeningScreen from '../components/openingscreen/RegularOpeningScreen';

export default {
  name: 'OpeningScreen',
  components: {
    RegularOpeningScreen,
    MobileOpeningScreen,
  },
};
</script>

<style scoped>

</style>
