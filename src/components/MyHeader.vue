<template>
  <header>
    <MyHeaderTop :contacts="contacts"/>
    <MyHeaderBottom/>
  </header>
</template>

<script>
import MyHeaderTop from './MyHeaderTop.vue';
import MyHeaderBottom from './MyHeaderBottom.vue';
export default {
  name: "MyHeader",
  components: { 
    MyHeaderTop,
    MyHeaderBottom
  },
  props: {
    contacts: Object
  }
}
</script>

<style lang="scss">
</style>