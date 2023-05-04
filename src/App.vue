<script>
    import HeaderComp from './components/HeaderComp.vue';
    import Thumb from './components/Thumb.vue';
    import BlueNav from './components/BlueNav.vue';
    import jumbotron from './components/jumbotron.vue';
    import preFooter from './components/preFooter.vue';
    import footerComp from './components/footerComp.vue';

    export default {
      name: 'App',
      components: {
        HeaderComp,
        Thumb,
        BlueNav,
        jumbotron,
        preFooter,
        footerComp,
      }
    }
</script>

<template>
  <HeaderComp/>
  <main>
    <jumbotron/>
    <Thumb/>
    <BlueNav/>
    <preFooter/>
    <footerComp/>
  
  </main>

</template>

<style lang="scss">
// @use './style/partials/_variables.scss' as *;
@use "./style/main.scss" as *;

</style>

