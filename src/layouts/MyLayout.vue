<template>
  <q-layout view="hHh Lpr lff" class="bg-dark">
    <!-- <q-header elevated class="">
      <q-toolbar>
        <q-toolbar-title class="absolute-center">
          Portfolio and Resume
        </q-toolbar-title>
      </q-toolbar>
    </q-header> -->

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MyLayout',

  data () {
    return {
    }
  }
}
</script>
