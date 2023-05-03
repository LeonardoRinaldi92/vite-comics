<script>
    import HeaderComp from './components/HeaderComp.vue';
    import Thumb from './components/Thumb.vue';
    import BlueNav from './components/BlueNav.vue';

    export default {
      name: 'App',
      components: {
        HeaderComp,
        Thumb,
        BlueNav,
      }
    }
</script>

<template>
  <HeaderComp/>
  <main>
    <Thumb/>
    <BlueNav/>
  
  </main>

</template>

<style lang="scss">
// @use './style/partials/_variables.scss' as *;
@use "./style/main.scss" as *;

</style>

