<template>
  <q-layout view="hHh lpR fFf" class="bg-website-white">
      <q-header
        elevated
        class="bg-primary text-white"
        height-hint="98"
      >
        <q-toolbar class="bg-white text-dark">
          <q-toolbar-title >
            <q-avatar style="width:80px; height: 80px">
              <img src="../statics/HonoluluBakingCircle.png">
            </q-avatar>
            Honolulu Baking Company
          </q-toolbar-title>
          <q-tabs align="right">
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
