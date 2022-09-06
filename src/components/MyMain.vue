<template>
  <main>
    <MyWhoWeAre/>
    <MyServices/>
    <MyLogistical/>
    <MyResults/>
    <MyFeedback/>
  </main>
</template>

<script>
  import MyWhoWeAre from './MyWhoWeAre.vue';
  import MyServices from './MyServices.vue';
import MyLogistical from './MyLogistical.vue';
import MyResults from './MyResults.vue';
import MyFeedback from './MyFeedback.vue';
  export default {
    name: "MyMain",
    components: {
    MyWhoWeAre,
    MyServices,
    MyLogistical,
    MyResults,
    MyFeedback
}
  }
</script>

<style lang="scss">

</style>