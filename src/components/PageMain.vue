<script>
    import AppDreamSection from './AppDreamSection.vue';
    import AppCourses from './AppCourses.vue';
    import AppContacts from './AppContacts.vue'
    export default {
        name: 'PageMain',
        components: {
            AppDreamSection,
            AppCourses,
            AppContacts
        },
        data() {
            return {
                events: [
                    {
                        where: 'Texas, US',
                        title: 'Storytelling Workshop',
                        day: 22,
                        month: 'NOV'
                    },
                    {
                        where: 'New York, US',
                        title: 'Painting Art Contest 2024',
                        day: 10,
                        month: 'OCT'
                    },
                    {
                        where: 'Hamburg, Germany',
                        title: 'International Art Fair 2024',
                        day: 23,
                        month: 'NOV'
                    },
                    {
                        where: 'Illinois, US',
                        title: 'Street Performance: Call for Artist',
                        day: 15,
                        month: 'DEC'
                    },
                    {
                        where: 'Illinois, US',
                        title: 'Consumer Food Safety Education Conference',
                        day: 22,
                        month: 'JUL'
                    },
                    {
                        where: 'Dubai',
                        title: 'How meditation improve your mental health?',
                        day: 12,
                        month: 'AUG'
                    },
                ],
            };
        }
    }
</script>


<template>
    <AppDreamSection></AppDreamSection>
    <AppCourses></AppCourses>
    <AppContacts></AppContacts>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
</style>