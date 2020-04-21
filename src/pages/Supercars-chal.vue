<template>
  <q-page>
    <div class="fit row  justify-center items-center content-center">
      <h3>Supercars Challenge</h3>
    </div>
    <div class="full-width row  justify-center items-start content-center">
      <iframe
      src="https://docs.google.com/spreadsheets/d/e/2PACX-1vScq581A4vug5n3oQ3K5XGek5ftvUXNo9tW798eh_SRwiKZ0XfDLSkoeu2pR2YH2H8OfCysSme91rj_/pubhtml?gid=200402505&amp;single=true&amp;widget=true&amp;headers=false"
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