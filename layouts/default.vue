<template>
  <div>
    <header>
    <TopNavigation/>
    <MainNavigation/>
    </header>
    <div id="app" class="container site main p-md-0">
    <Nuxt />
    </div>
    <div class="container-fluid footer-container aside-stopper p-0">
    <Footer />
    </div>
  </div>
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

