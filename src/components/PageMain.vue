<script>
    import AppDreamSection from './AppDreamSection.vue';
    import AppCourses from './AppCourses.vue';
    export default {
        name: 'PageMain',
        components: {
            AppDreamSection,
            AppCourses
        }
    }
</script>


<template>
    <AppDreamSection></AppDreamSection>
    <AppCourses></AppCourses>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
</style>