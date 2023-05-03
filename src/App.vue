<script>
    import HeaderComp from './components/HeaderComp.vue';
    import Thumb from './components/Thumb.vue'

    export default {
      name: 'App',
      components: {
        HeaderComp,
        Thumb,
      }
    }
</script>

<template>
  <HeaderComp/>
  <main>
    <Thumb/>
  </main>

</template>

<style lang="scss">
// @use './style/partials/_variables.scss' as *;
@use "./style/main.scss" as *;

</style>

