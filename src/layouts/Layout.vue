<template>
  <div>
    <q-layout class="bg-website-white" view="hHh lpR fFf">
      <q-header
        elevated
        class="text-white"
        height-hint="98"
      >
        <q-toolbar
          class="bg-website-white text-dark"
          style="font-family: Satisfy, cursive; height: 20px;"
        >
          <q-toolbar-title>
            Honolulu Baking Company
          </q-toolbar-title>
          <q-tabs
            alight-left
            class="text-dark"
            style="font-family: Satisfy, cursive;"

          >
            <q-route-tab to="/page1" name="About Us">
              <div class="text-weight-bold">ABOUT US</div>
            </q-route-tab>
            <q-route-tab to="/page2" name="Contacts">
              <div class="text-weight-bold">CONTACTS</div>
            </q-route-tab>
            <q-route-tab to="/page3" name="Clients">
              <div class="text-weight-bold">CLIENTS</div>
            </q-route-tab>
          </q-tabs>
        </q-toolbar>

      </q-header>

      <q-page-container>
        <router-view />
      </q-page-container>

    </q-layout>
  </div>
</template>

<script>
export default {
  name: 'Layout',
  data() {
    return {
    };
  },
};
</script>

<style scoped>

</style>
