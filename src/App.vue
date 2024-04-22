<script>
  import PageHeader from './components/PageHeader.vue';
  export default {
    components: {
      PageHeader
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
</template>


<style lang="scss">
@use './style/generic';
</style>