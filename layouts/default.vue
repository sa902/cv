<template>
  <v-app dark :style="{background: '#F1FAEE'}">

    <v-main>

        <nuxt />
    </v-main>

    <v-footer
      :absolute="!fixed"
      :style="{background: '#457B9D'}"
      app
    >
      <span>&nbsp</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
<style media="screen">

</style>
