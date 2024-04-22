<script>
    export default {
        name: 'AppDreamSection'
    }
</script>


<template>
    <div class="container">
        <div class="ms-title-container text-center my-5 pt-3">
            <small>START LEARNING CODING LANGUAGES</small>
            <div class="fs-1">
                <span class="ms-dream">Build Your Dream </span><span class="ms-today">TODAY</span>
            </div>
        </div>
        <!-- Sezione con cards -->
        <div class="row mt-5 pt-5">
            <div class="col-3">
                <div class="ms-card mt-2">
                    <div class="img-container">
                        <img src="../assets/img/home-5-image-box-01.png" alt="...">
                    </div>
                    <div class="text-center ms-text">
                        <h5 class="card-title">Idea Discussion</h5>
                        <p class="card-text py-4">Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
                        <button class="ms-btn">Start Now <i class="fa-solid fa-arrow-right ps-3"></i></button>
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="ms-card mt-2">
                    <div class="img-container">
                        <img src="../assets/img/home-5-image-box-02.png" alt="...">
                    </div>
                    <div class="text-center ms-text">
                        <h5 class="card-title">Web Development</h5>
                        <p class="card-text py-4">Learn to start building a webpage from scratch. You decide your own pace, course and speed.</p>
                        <button class="ms-btn">Start Now <i class="fa-solid fa-arrow-right ps-3"></i></button>
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="ms-card mt-2">
                    <div class="img-container">
                        <img src="../assets/img/home-5-image-box-03.png" alt="...">
                    </div>
                    <div class="text-center ms-text">
                        <h5 class="card-title">System Administration</h5>
                        <p class="card-text py-4">Learners are encouraged to study the mechanism and structure of system administration .</p>
                        <button class="ms-btn">Start Now <i class="fa-solid fa-arrow-right ps-3"></i></button>
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="ms-card mt-2">
                    <div class="img-container">
                        <img src="../assets/img/home-5-image-box-04.png" alt="...">
                    </div>
                    <div class="text-center ms-text">
                        <h5 class="card-title">Graphic Design</h5>
                        <p class="card-text py-4">Have a passion for graphic and arts? Show your talents with confidence and self-assertiveness.</p>
                        <button class="ms-btn">Start Now <i class="fa-solid fa-arrow-right ps-3"></i></button>
                    </div>
                </div>
            </div>
        </div>
        <!-- Sezione con ragazzo che esulta -->
        <div class="row mt-5 pt-5">
            <div class="col-6"></div>
            <div class="col-6"></div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;
.ms-title-container{

    .ms-dream{
        color: $purple;
    }
    .ms-today{
        color: $green;
    }

}
.img-container{
    width: 250px;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: self-start;
    img{
        max-width: 100%;
    }
}

.ms-btn{
    border: none;
    background-color: white;
    color: $light-purple;
    padding: 8px 40px;

    &:hover{
        color: $green;
        background-color: $light-gray;
        border-radius: 5px;
    }
}
.ms-text{
    p{
        color: $gray;
    }
}
</style>