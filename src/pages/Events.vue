<template>
  <q-page>
    <div class="fit row  justify-center items-center content-center">
      <h3>Events</h3>
    </div>
    <div class="full-width row  justify-center items-start content-center">
      <div class="col shadow-1 q-gutter-sm">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" style="max-width: 300px">
        <div class="absolute-bottom text-subtitle1 text-center">
          Caption
        </div>
      </q-img>
      </div>
      <div class="col shadow-1 q-gutter-sm">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" style="max-width: 300px">
        <div class="absolute-bottom text-subtitle1 text-center">
          Caption2
        </div>
      </q-img>
      </div>
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