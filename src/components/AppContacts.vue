<script>
    export default {
        name: 'AppContacts'
    }
</script>


<template>
    <!-- Sezione con eventi -->
    <section>
        <div class="container">
            <div class="ms-title-wrapper text-center py-5">
                <small class="ms-thin ms-small">GET IN CONTACT NOW</small>
                <h2 class="ms-purple py-4">Upcoming <span class="ms-green">Events</span></h2>
            </div>
        </div>
    </section>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
/* STILI */
.ms-green{
    color: $green;
}
.ms-purple{
    color: $purple;
}
.ms-thin{
    font-weight: 300;
}
.ms-small{
    font-size: 12px;
}
</style>