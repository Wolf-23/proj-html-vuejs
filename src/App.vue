<template>
  <div id="app">
    <MyHeader :contacts="contacts"/>
    <MyMain :contacts="contacts"/>
    <MyFooter :contacts="contacts"/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  },
  data() {
    return {
      contacts: {
        clock: {
              icon: 'fa-solid fa-clock',
              text: 'Open Hours: Mon - Sat - 9:00 - 18:00'
          },
        phone: {
            icon: 'fa-solid fa-phone',
            text: '+1 (305) 1234-5678'
          },
        email: {
            icon: 'fa-solid fa-envelope',
            text: 'hello@example.com'
          },
        maps: {
            icon: 'fa-solid fa-location-dot',
            text: 'Main Avenue, 987'
          },
        }
    }
  }
      
  }
</script>

<style lang="scss">
  @import '~@fortawesome/fontawesome-free/css/all.css';
  @import '../src/styles/general.scss';
  @import '../src/styles/vars.scss';
  @import '../src/styles/styles.scss';

</style>
