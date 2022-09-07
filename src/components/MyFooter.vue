<template>
  <footer>
    <MyFooterTop :contacts="contacts"/>
    <MyFooterBottom/>
  </footer>
</template>

<script>
  import MyFooterTop from './MyFooterTop.vue';
  import MyFooterBottom from './MyFooterBottom.vue';
  export default {
    name: "MyFooter",
    components: { 
      MyFooterTop, 
      MyFooterBottom 
    },
    props: {
      contacts: Object
    }
  }
</script>

<style lang="scss">

</style>