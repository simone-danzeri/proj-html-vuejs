<script>
    export default {
        name: 'AppHero',
    }
</script>


<template>
    <div class="ms-bg">
        <div class="container">
            <div class="row py-5">
                <div class="col-6">
                    <div class="ms-card">
                        <h1>Complete Your Dreams In JavaS Programming</h1>
                        <p class="py-4">Learn any coding program in distance and for a reasonable fee. You don't have to struggle alone, you've got our assistance and help.</p>
                        <button> <i class="fa-solid fa-download pe-3"></i> Download free E-Book</button>
                    </div>
                </div>
                <div class="col-6">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa saepe doloribus ducimus dolore quidem vitae qui ab amet tempore numquam quae blanditiis pariatur neque expedita quod, perspiciatis officiis iste odio!</div>
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
    width: 100%;
    height: 400px;

    .ms-card{
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
}
</style>