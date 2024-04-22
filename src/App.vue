<script>
  import PageHeader from './components/PageHeader.vue';
  import AppHero from './components/AppHero.vue';
  import PageMain from './components/PageMain.vue';
  export default {
    components: {
      PageHeader,
      AppHero,
      PageMain
    },
    data() {
      return {
        navLinks: [
          'Home',
          'Pages',
          'Courses',
          'Features',
          'Blog',
          'Shop'
        ],
      }
    }
  }
</script>


<template>
  <PageHeader :navBar="navLinks"></PageHeader>
  <AppHero></AppHero>
  <PageMain></PageMain>
</template>


<style lang="scss">
@use './style/generic';
</style>