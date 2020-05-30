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
      <q-space/>
      <transition
        mode="out-in"
        appear-active-class="animated fadeIn"
        leave-active-class="animated fadeOut"
        :duration="350"
      >
        <router-view
          class="fixed-center"
        />
      </transition>
      <q-space/>
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
