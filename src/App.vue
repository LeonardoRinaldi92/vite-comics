<script>
    import HeaderComp from './components/HeaderComp.vue';

    export default {
      name: 'App',
      components: {
        HeaderComp,
      }
    }
</script>

<template>
  <div id="title">
    <HeaderComp/>
  </div>
</template>

<style lang="scss">
// @use './style/partials/_variables.scss' as *;
@use "./style/main.scss" as *;

</style>

