<script>
    export default {
        name: 'AppHero',
    }
</script>


<template>
    <div class="ms-bg">
        <div class="ms-side d-flex flex-column justify-content-center align-items-center gap-3 ">
            <i class="fa-solid fa-ruler-combined"></i>
            <i class="fa-solid fa-life-ring"></i>
            <i class="fa-solid fa-book"></i>
            <i class="fa-solid fa-cart-shopping"></i>
        </div>
        <div class="container">
            <div class="row py-5">
                <div class="col-6">
                    <div class="ms-card d-flex flex-column justify-content-center">
                        <h1>Complete Your Dreams In JavaS Programming</h1>
                        <p class="py-4">Learn any coding program in distance and for a reasonable fee. You don't have to struggle alone, you've got our assistance and help.</p>
                        <button> <i class="fa-solid fa-download pe-3"></i> Download free E-Book</button>
                    </div>
                </div>
                <div class="col-6">
                    <div class="ms-img-container">
                        <img src="../assets/img/home-5-hero-image.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
.ms-bg{
    background-image: url('../assets/img/jumbo-overlay.svg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    width: 100%;
    position: relative;
    

    .ms-side{
        position: absolute;
        top: 20%;
        right: 0;
        background-color: white;
        padding: 9px 8px;
        border-radius: 5px;

    }

    .ms-card{
        height: 100%;

        h1{
            width: 60%;
            color: $purple;
        }

        p{
            width: 63%;
            color: $light-purple;
        }

        button{
            background-color: $green;
            border: none;
            color: white;
            padding: 12px 14px;
            border-radius: 5px;
            font-size: 14px;
            width: 250px;

            &:hover{
                background-color: $purple;
            }
        }
    }

    .ms-img-container{
        width: 80%;

        img{
            max-width: 100%;
        }
    }
}
</style>