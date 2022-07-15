<template>
  <div id="app">
    <MyHeader :dataHeader="this.dataHeader" />
  </div>
</template>

<script>
import MyHeader from './components/myHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
  },
  data() {
    return {
      dataHeader: {
        hours: 'Open Hours: Mon-Sat - 9:00 - 18:00',
        telephone: '+1 (305) 1234-5678',
        mail: 'hello@example.com',
        // Icone non funzionante tramite props. Riprovare Lunedì, inserite staticamente
        icon: {
          facebook: '',
          linkedin: '',
          twitter: '',
        },
        allNav: [

          {
            nav: 'HOME',
          },
          {
            nav: 'ABOUT',
          },
          {
            nav: 'SERVICES',
          },
          {
            nav: 'PRICING',
          },
          {
            nav: 'BLOG',
          },

        ],
        subtext: 'Successful strategies require data analysis, creativity and customer focus, taking advantage of the latest technologies to offer excellent services.'



      },
    }
  }
}
</script>

<style lang="scss">
@import 'bootstrap';
@import './style/common.scss';
</style>
