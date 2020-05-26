<template>
  <div class="q-gutter-sm absolute-center">
    <q-card class="main-card row">
      <div class="col-7">
        <q-card-section class="col-12">
          <div class="text-h5">
            <q-icon name="fas fa-address-card"/> Resume and Portfolio
          </div>
        </q-card-section>
        <q-card-section>
          <div>
            Name
          </div>
        </q-card-section>
        <q-card-section>
          <div>
            Contact
          </div>
        </q-card-section>
        <q-card-section>
          <div>
            Intro
          </div>
        </q-card-section>
        <q-card-section>
          <div>
            Instructions
          </div>
        </q-card-section>
        <q-card-actions class="absolute-bottom">
          <q-btn
            v-for="(btn, index) in buttonLabels"
            dense
            :key="index"
            :label="btn.label"
            :icon="btn.icon"
            flat
          />
        </q-card-actions>
      </div>
      <div class="col-5">
        Information goes here
      </div>
    </q-card>
  </div>
</template>

<script>
export default {
  name: 'PageIndex',

  data () {
    return {
      buttonLabels: [
        {
          label: 'Skills',
          icon: 'fas fa-vial',
          method: ''
        },
        {
          label: 'Work History',
          icon: 'fas fa-file-contract',
          method: ''
        },
        {
          label: 'Projects',
          icon: 'fas fa-tools',
          method: ''
        },
        {
          label: 'Education',
          icon: 'fas fa-book-open',
          method: ''
        }
      ]
    }
  }
}
</script>

<style lang="sass">
  .main-card
    min-width: 800px
    min-height: 400px
</style>
