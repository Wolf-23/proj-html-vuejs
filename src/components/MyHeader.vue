<template>
  <header>
    <MyHeaderTop/>
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
    }
}
</script>

<style lang="scss">
</style>