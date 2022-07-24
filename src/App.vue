<template>
  <div id="app">
    <MyHeader :dataHeader="this.dataHeader" />
    <MyMain />
    <MyFooter :dataFooter="this.dataFooter" :dataHeader="this.dataHeader" />
  </div>
</template>

<script>
import MyHeader from './components/myHeader.vue';
import MyMain from './components/myMain.vue';
import MyFooter from './components/myFooter.vue';


export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  },
  data() {
    return {
      dataHeader: {
        hours: 'Open Hours: Mon-Sat - 9:00 - 18:00',
        telephone: '+1 (305) 1234-5678',
        mail: 'hello@example.com',
        icons: [
          {
            icon: "fa-facebook-f",
          },
          {
            icon: "fa-twitter",
          },
          {
            icon: "fa-linkedin-in",
          },
        ],
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
      dataFooter: {
        preFixLogo: 'NEX',
        logo: 'GEN ',
        text: 'A Functional HTML Template for corporate & Business',
        icon1: 'fa-phone',
        location: 'Main Avenue, 987',
        icon2: 'fa-envelope',
        icon3: 'fa-location-dot',
        button: 'GET IN TOUCH',
        title1: 'About',
        title2: 'Services',
        title3: 'Support',
        footerBottomText: 'Enjoy  the low price. We are tracking any intention of piracy',
        footerBottomText2: '© 2020 NEXGEN is proudly Powered by ' ,
        footerBottomText3: 'Codings.',
        about: [
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'The Company',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Institutional',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Social & Events',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Innovation',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Environment',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Technology',
          },
        ],
        services: [
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Audit & Assurance',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Financial Advisory',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Analytics M&A',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Middle Marketing',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Legal Consulting',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Regulatory Risk',
          },
        ],
        support: [
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Responsibility',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Terms of Use',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'About Cookie',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Privacy Policy',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Accessibility',
          },
          {
            // <font-awesome-icon icon="fa-solid fa-chevron-right" />
            icon: 'fa-chevron-right',
            text: 'Information',
          },
        ]
      },
    }
  }
}
</script>

<style lang="scss">
@import 'bootstrap';
@import './style/common.scss';
</style>
