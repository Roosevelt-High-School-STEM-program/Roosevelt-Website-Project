<template>
  <q-layout view="hHh lpR fFf" class="bg-website-white">
      <q-header
        elevated
        class="bg-primary text-white"
        height-hint="98"

      >
        <q-toolbar class="bg-website-mustard-yellow text-dark">
          <q-toolbar-title >
            <q-avatar>
              <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
            </q-avatar>
            Honolulu Baking Company
          </q-toolbar-title>
          <q-tabs align="right" class="bg-website-mustard-yellow">
            <q-route-tab to="/page1" label="About Us" />
            <q-route-tab to="/page2" label="Contacts" />
            <q-route-tab to="/page3" label="Clients" />
          </q-tabs>
        </q-toolbar>

      </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  data() {
    return {
    };
  },
};
</script>

<style scoped>

</style>
