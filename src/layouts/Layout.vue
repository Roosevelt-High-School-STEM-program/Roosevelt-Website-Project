<template>
  <div>
    <q-layout view="hHh lpR fFf" style="background-color: #424C55">
      <q-header
        elevated
        class="text-white"
        height-hint="98"
      >
        <q-toolbar class=" text-white" style="background-color: #424C55">
          <q-toolbar-title >
            <!--            <q-avatar style="width:80px; height: 80px">-->
            <!--              <img src="../statics/HonoluluBakingCircle.png">-->
            <!--            </q-avatar>-->
            Honolulu Baking Company
          </q-toolbar-title>
          <q-btn dense flat round class="float-left" icon="menu" @click="left = !left" />
        </q-toolbar>
      </q-header>
        <q-drawer
          overlay
          v-model="left"
          side="left"
          :width="200"
          :breakpoint="200"
          elevated
        >
          <q-tabs alight-left vertical>
            <q-route-tab to="/page1" label="About Us" />
            <q-route-tab to="/page2" label="Contacts" />
            <q-route-tab to="/page3" label="Clients" />
          </q-tabs>
        </q-drawer>

      <q-page-container>
        <router-view />
      </q-page-container>

    </q-layout>
  </div>
</template>

<script>
export default {
  data() {
    return {
      left: false,
    };
  },
};
</script>

<style scoped>

</style>
