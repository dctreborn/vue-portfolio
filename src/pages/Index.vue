<template>
  <div>
    <q-card class="main-card row">
      <div class="col-6">
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
            size="sm"
            dense
            :key="index"
            :label="btn.label"
            :icon="btn.icon"
            flat
            @click="navigate(btn.path)"
          />
        </q-card-actions>
      </div>
      <q-card-section class="col-6">
        <q-scroll-area class="info-area">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ultrices ultricies nunc ut sollicitudin. Donec ac nibh id turpis malesuada semper a in lectus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean ut sapien sodales arcu lacinia vehicula. Pellentesque eget neque dictum, iaculis augue ut, mollis nibh. Morbi ornare luctus lacus. Cras commodo augue malesuada, egestas nibh sed, auctor nulla. Nulla eget elit ipsum. Suspendisse ac aliquet dui. Vivamus eget tempus nisi.

            Vestibulum vel nulla ac urna accumsan varius id non lorem. Ut faucibus nunc eu placerat commodo. Nam sit amet diam augue. Donec a metus lobortis, bibendum nibh nec, luctus nisi. Vestibulum mattis sagittis enim, et facilisis orci posuere congue. In vitae sodales augue. Fusce lectus mauris, tristique ullamcorper est quis, suscipit ornare massa. Nunc et bibendum turpis, eu mattis mi. Duis ac enim sit amet nulla porta efficitur. Sed eleifend diam vel risus congue, vitae mattis orci lacinia. Vivamus magna enim, tempus ac urna ut, blandit dapibus diam. Maecenas finibus sagittis velit eu efficitur. Morbi tempor sodales ipsum ac ultrices. In tempor lacus eget pellentesque placerat. Fusce non interdum massa, vulputate mollis massa.

            Integer vitae consectetur nisl. In lobortis tellus eros, sed iaculis felis tincidunt ac. Vestibulum consequat tellus magna, vel aliquam nibh ultrices eleifend. Praesent porttitor convallis lacinia. Aliquam id aliquam dui. Curabitur mauris justo, condimentum sed bibendum egestas, vehicula eget urna. Aliquam dictum sapien vel est tincidunt vehicula. Curabitur dignissim elit tellus, quis placerat velit aliquam ut.

            Mauris massa dolor, mollis eu nisi vel, semper finibus orci. In hac habitasse platea dictumst. In hac habitasse platea dictumst. Etiam tempus felis posuere, rhoncus justo at, fringilla justo. Suspendisse molestie odio euismod vehicula mattis. Aenean porta nulla a urna lacinia iaculis. Fusce eget diam ut diam cursus ullamcorper. Sed ullamcorper turpis nec lacinia sollicitudin. Vestibulum eleifend, neque bibendum vestibulum hendrerit, purus urna vehicula nisi, a ornare purus lacus et augue. Phasellus molestie quis augue sed scelerisque. Fusce in velit ut nunc scelerisque interdum vitae sit amet lectus. Pellentesque dictum, nibh mattis egestas scelerisque, massa libero posuere tellus, non rhoncus erat urna sit amet quam. Donec diam sapien, dapibus a purus eu, sollicitudin aliquet quam. Sed dignissim facilisis magna ullamcorper cursus.

            Donec mattis enim odio, a faucibus lectus finibus vel. Etiam vitae ante vitae augue malesuada semper. Quisque est enim, volutpat at neque in, finibus maximus turpis. Nulla vehicula magna eget nibh accumsan, id placerat ipsum elementum. Sed tempor nulla eu justo egestas aliquam. Praesent non turpis ipsum. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
        </q-scroll-area>
      </q-card-section>
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
          path: 'terminal'
        },
        {
          label: 'Work History',
          icon: 'fas fa-file-contract',
          path: 'inventory'
        },
        {
          label: 'Projects',
          icon: 'fas fa-tools',
          path: ''
        },
        {
          label: 'Education',
          icon: 'fas fa-book-open',
          path: ''
        }
      ]
    }
  },

  methods: {
    navigate (path) {
      this.$router.push(`/${path}`)
    }
  }
}
</script>

<style lang="sass">
  .main-card
    min-width: 800px
    height: 450px

  .info-area
    height: 100%
    width: 100%
</style>
