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
        <div class="row justify-content-between my-5 pt-5">
            <div class="col-5">
                <div class="ms-img-container d-flex justify-content-end">
                    <img class="ms-man" src="../assets/img/about-us-03-image-01.png" alt="">
                </div>
            </div>
            <div class="col-5">
                <p>DREAM WITH <span class="ms-gray">MAXCOACH</span></p>
                <h1 class="mb-5">Construct A <span class="ms-green">Stunning</span> Career Perspective</h1>
                <div class="ms-accordion-title-container ms-first d-flex justify-content-between py-3 px-4">
                    <span>Multiple Platforms Supported for Teaching & Studying</span>
                    <span><i class="fa-solid fa-circle-minus"></i></span>
                </div>
                <div class="ms-accordion-text">
                    <p>
                        MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via material downloads. We know things aren't supposed to be devaured in a short time, you can always access our knowledge base from any device.
                    </p>
                </div>
                <div class="ms-accordion-title-container-2 d-flex justify-content-between py-3 px-4">
                    <span class="ms-accordion-title">Multiple Course Partecipation At The Same Time</span>
                    <span class="ms-accordion-fa"><i class="fa-solid fa-circle-plus"></i></span>
                </div>
                <div class="ms-accordion-title-container-2 d-flex justify-content-between py-3 px-4 mt-4">
                    <span class="ms-accordion-title">Multiple Course Partecipation At The Same Time</span>
                    <span class="ms-accordion-fa"><i class="fa-solid fa-circle-plus"></i></span>
                </div>
            </div>
        </div>
    </div>
            <!-- Sezione colorata con numeri -->
            <div class="row justify-content-around ms-bg-lightgray my-5 py-4">
            <div class="col-2 ps-5">
                <h3 class="ms-color-green">1.926</h3>
                <small>FINISHED SESSION</small>
            </div>
            <div class="col-2">
                <h3 class="ms-color-green">3.092+</h3>
                <small>ENROLLED LEARNERS</small>
            </div>
            <div class="col-2">
                <h3 class="ms-color-green">200</h3>
                <small>ONLINE INSTRUCTORS</small>
            </div>
            <div class="col-2 pe-5">
                <h3 class="ms-color-green">100%</h3>
                <small>SATISFACTION RATE</small>
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

.ms-img-container{
    height: 550px;
}

.ms-gray{
    color: $gray;
    font-weight: 700;
}

.ms-green{
    color: $green;
    font-weight: 300;
}

.ms-accordion-title-container{
    border-radius: 5px;
}
.ms-first{
    background-color: $green;
    color: white;
}

.ms-accordion-text{
    padding: 20px 12px;
    width: 80%;
    background-color: white;
}

.ms-accordion-title-container-2{
    border-radius: 5px;
    color: $gray;
    box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
    -webkit-box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
    -moz-box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
}


.ms-bg-lightgray{
    background-color: $light-gray;
    small{
        font-size: 12px;
        font-weight: 200;
    }
}
.ms-color-green{
    color: $green;
}
</style>