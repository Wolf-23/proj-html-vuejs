<template>
  <main>
    <MyWhoWeAre/>
    <MyServices/>
    <MyLogistical/>
  </main>
</template>

<script>
  import MyWhoWeAre from './MyWhoWeAre.vue';
  import MyServices from './MyServices.vue';
import MyLogistical from './MyLogistical.vue';
  export default {
    name: "MyMain",
    components: {
    MyWhoWeAre,
    MyServices,
    MyLogistical
}
  }
</script>

<style lang="scss">

</style>