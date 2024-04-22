<script>
    export default {
        name: 'PageHeader',
        data() {
            return {

            };
        },
        props: {
            navBar: Array
        }
    }
</script>


<template>
    <header class="ms-bg">
        <div class="container mt-2 d-flex align-items-center justify-content-between">
            <div class="ms-logo-container">
                <img class="ms-logo" src="../assets/img/dark-logo.png" alt="">
            </div>
            <div class="ms-nav-container d-flex">
                <div class="ms-links d-flex align-items-center">
                    <span v-for="link in navBar">{{ link }} <i class="fa-solid fa-caret-down"></i></span>
                </div>
                <div class="ms-nav-icons d-flex align-items-center gap-2 ms-5 me-3">
                    <i class="fa-solid fa-cart-shopping"></i>
                    <i class="fa-solid fa-circle-user"></i>
                </div>
                <div class="ms-search-bar">
                    <nav class="navbar">
                        <div class="container-fluid">
                            <form class="d-flex" role="search">
                            <input type="search" placeholder="Search..." aria-label="Search">
                            <button type="submit"> <i class="fa-solid fa-magnifying-glass"></i> </button>
                            </form>
                        </div>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
.ms-bg{
    background-color: $light-gray;
}
.ms-logo-container{
    .ms-logo{
        width: 175px;
    }
}

.ms-nav-container{
    .ms-links{
        gap: 30px;
        color: $light-purple;
    }
    input{
        height: 50px;
        width: 150px;
        border: none;
        padding-left: 20px;
    }
    button{
        background-color: white;
        color: green;
        border: none;
        padding-right: 20px;
        cursor: pointer;
    }
}
</style>