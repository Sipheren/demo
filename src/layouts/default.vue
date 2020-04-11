<template>
  <q-layout view="hHh Lpr fFf"> <!-- Be sure to play with the Layout demo on docs -->

    <!-- (Optional) The Header -->
    <q-header elevated class="row justify-center">
      <q-toolbar class="col">
      <img src="http://sipheren.com/logo.png" style="max-width: 20%">
      </q-toolbar>

      <q-tabs>
        <q-route-tab to="/" label="Home"/>
        <q-route-tab to="Calendar" label="Calendar"/>
        <q-route-tab to="Rules" label="Rules"/>
      </q-tabs>
      
    </q-header>

    <q-page-container>
      <!-- This is where pages get injected -->
      <router-view :key="$route.params.id" />
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  // name: 'LayoutName',

  data () {
    return {
      leftDrawer: true
    }
  }
}
</script>
