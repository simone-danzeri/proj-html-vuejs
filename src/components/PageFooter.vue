<script>
    export default {
        name: 'PageFooter',
        props: {
            exploreLinks: Array,
            storyLinks: Array,
            informationLinks: Array
        }
    }
</script>


<template>
    <div class="container">
        <div class="ms-footer-container d-flex justify-content-between">
            <div class="ms-address">
                <ul>
                    <li class="fw-bold pb-4">Address</li>
                    <li class="fw-lighter">38 NE 191st St #87394 Miami, FL 3317-6531</li>
                    <li class="fw-lighter py-4">+1 (305) 547-7734 (9am - 5pm EST, Monday - Friday)</li>
                    <li class="fw-lighter">support@maxcoach.com</li>
                    <li class="pt-5">
                        <ul class="d-flex gap-5 ms-text-gray">
                            <li><i class="fa-brands fa-facebook fs-3"></i></li>
                            <li><i class="fa-brands fa-twitter fs-3"></i></li>
                            <li><i class="fa-brands fa-linkedin fs-3"></i></li>
                            <li><i class="fa-brands fa-instagram fs-3"></i></li>
                        </ul>
                    </li>
                </ul>
            </div>
            <div class="ms-links d-flex">
                <ul>
                    <li class="fw-bold pb-2">Explore</li>
                    <li v-for="eachLink in exploreLinks" class="fw-lighter py-2">{{ eachLink }}</li>
                </ul>
                <ul class="pe-4 ">
                    <li class="text-white pb-2">Story</li>
                    <li v-for="eachLink in storyLinks" class="fw-lighter py-2">{{ eachLink }}</li>
                </ul>
                <ul>
                    <li class="fw-bold pb-2">Information</li>
                    <li v-for="eachLink in informationLinks" class="fw-lighter py-2">{{ eachLink }}</li>
                </ul>
            </div>
        </div>
        <div class="text-center">
            <small class="ms-text-gray fw-light"><i class="fa-regular fa-copyright"></i>  2024 Maxcoach. All Rights Reserved.</small>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
.ms-text-gray{
    color: $gray;
}
.ms-footer-container{
    padding: 100px 0px;
    ul{
        list-style: none;
    }
}
</style>