<template>
  <q-page class="flex flex-center">
    <div>
      <div class="flex flex-center q-my-md">
        <!-- <input type="checkbox"> -->
        <input type="checkbox" v-model='mode' @change="changeMode(mode)">
      </div>
      <div class="flex flex-center q-my-lg">
        <div class="q-mx-md foto"><span>Lorem Ipsum</span></div>
      </div>
      <div class="flex q-my-md">
        <a href="#" class="q-mx-md btn-link"><span><i class="fab fa-github-alt"></i></span></a>
        <a href="#" class="q-mx-md btn-link"><span><i class="fab fa-linkedin-in"></i></span></a>
        <a href="#" class="q-mx-md btn-link"><span><i class="fab fa-instagram"></i></span></a>
      </div>
      <div class="flex flex-center q-my-lg">
        <div class="q-mx-md email"><span>lucyjbrandao@gmail.com</span></div>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',

  data () {
    return {
      mode: false
    }
  },

  methods: {
    changeMode (mode) {
      this.$q.dark.set(mode)
    }
  }
}
</script>
