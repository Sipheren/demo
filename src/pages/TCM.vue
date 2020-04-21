<template>
  <q-page>
    <div class="fit row  justify-center items-center content-center">
      <h3>TCM</h3>
    </div>
    <div class="full-width row  justify-center items-start content-center">
      <iframe
      src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTFk6XMCLfGFlypZ20jCZA8puYPD5OAeWYkYascG-bEhleOdiuWCD61joqxQvfcaHYW2DGoxxVmMICD/pubhtml?gid=991861507&amp;single=true&amp;widget=true&amp;headers=false"
      frameborder="0" scrolling="yes" class="iframe-style" width="100%">
    </iframe>
    </div>
  </q-page>
</template>

<style>
.iframe-style {
  height: calc(99vh - 90px);
}
</style>

<script>
export default {
  name: 'PageIndex'
}
</script>