<script>
  import PageHeader from './components/PageHeader.vue';
  import AppHero from './components/AppHero.vue';
  import PageMain from './components/PageMain.vue';
  import PageFooter from './components/PageFooter.vue';
  export default {
    components: {
      PageHeader,
      AppHero,
      PageMain,
      PageFooter
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
        exploreLinks: [
          'Start here',
          'Blog',
          'About us'
        ],
        storyLinks: [
          'Success story',
          'Courses',
          'Contact us'
        ],
        informationLinks: [
          'Membership',
          'Purchase guide',
          'Privacy policy',
          'Terms of services'
        ],
      }
    }
  }
</script>


<template>
  <PageHeader :navBar="navLinks"></PageHeader>
  <AppHero></AppHero>
  <PageMain></PageMain>
  <PageFooter :exploreLinks="exploreLinks" :storyLinks="storyLinks" :informationLinks="informationLinks"></PageFooter>
</template>


<style lang="scss">
@use './style/generic';
</style>