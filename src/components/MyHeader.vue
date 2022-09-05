<template>
  <header>
    <MyHeaderTop/>
  </header>
</template>

<script>
import MyHeaderTop from './MyHeaderTop.vue';
export default {
    name: "MyHeader",
    components: { 
        MyHeaderTop 
    }
}
</script>

<style lang="scss">
    header {
        height: 100px;
        background-color: red;
    }
</style>