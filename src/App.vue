<script>
  import PageHeader from './components/PageHeader.vue';
  import AppHero from './components/AppHero.vue';
  export default {
    components: {
      PageHeader,
      AppHero
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
</template>


<style lang="scss">
@use './style/generic';
</style>