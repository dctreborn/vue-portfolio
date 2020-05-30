<template>
  <div>
    <q-card>
      <q-card-section>
        <q-btn label="Back" @click="goHome"/>
        Terminal
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {
  methods: {
    goHome () {
      this.$router.push('/')
    }
  }
}
</script>
