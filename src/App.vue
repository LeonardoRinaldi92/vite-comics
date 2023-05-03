<script>
    import HeaderComp from './components/HeaderComp.vue';
    import Thumb from './components/Thumb.vue';
    import BlueNav from './components/BlueNav.vue';
    import jumbotron from './components/jumbotron.vue';

    export default {
      name: 'App',
      components: {
        HeaderComp,
        Thumb,
        BlueNav,
        jumbotron,
      }
    }
</script>

<template>
  <HeaderComp/>
  <main>
    <jumbotron/>
    <Thumb/>
    <BlueNav/>
  
  </main>

</template>

<style lang="scss">
// @use './style/partials/_variables.scss' as *;
@use "./style/main.scss" as *;

</style>

