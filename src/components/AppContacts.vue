<script>
    export default {
        name: 'AppContacts',
        data() {
            return {

            };
        },
        props: {
            event: Object
        }
    }
</script>


<template>
    <!-- Sezione con eventi -->
    <section class="events">
        <div class="container">
            <!-- Titoli -->
            <div class="ms-title-wrapper text-center py-5">
                <small class="ms-thin ms-small">GET IN CONTACT NOW</small>
                <h2 class="ms-purple py-4">Upcoming <span class="ms-green">Events</span></h2>
            </div>
            <!-- Cards -->
            <div class="ms-cards-wrapper d-flex flex-wrap">
                <div class="ms-event-card d-flex justify-content-between" v-for="eachEvent in event">
                    <div class="ms-card-left ps-5">
                        <small class="ms-where"><i class="fa-solid fa-location-dot"></i> {{ eachEvent.where }} </small>
                        <h5 class="ms-title pt-2">{{ eachEvent.title }}</h5>
                    </div>
                    <div class="ms-card-right pe-5 d-flex flex-column align-items-center">
                        <div class="ms-day text-center">{{ eachEvent.day }}</div>
                        <div class="ms-month text-center">{{ eachEvent.month }}</div>
                        <div>
                            <button>Get Ticket</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="d-flex justify-content-center mt-4">
                <small class="ms-thin">Excited about our events? <a class="ps-2" href="#">View all events <i class="fa-solid fa-arrow-right ps-2"></i></a></small>
            </div>
        </div>
    </section>
    <!-- Sezione testimonials -->
    <section class="testimonials">
        <div class="container">
            <!-- Titoli -->
            <div class="ms-title-wrapper text-center py-5">
                <small class="ms-thin ms-small">PEOPLE ARE PRAISIN MAXCOACH</small>
                <h2 class="ms-purple py-4">What make they <span class="ms-green">Love Us?</span></h2>
            </div>
            <!-- Cards dei testimonials -->
            <div class="row d-flex justify-content-around mt-5 pt-3">
                <div class="col-3">
                    <div class="ms-testimonial-card d-flex flex-column align-items-center">
                        <div class="ms-pp-container">
                            <img class="pp" src="../assets/img/testimonial-avata-02.jpg" alt="">
                        </div>
                        <p>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
                        <h5>MINA HOLLACE</h5>
                        <small>/ Freelancer</small>
                    </div>
                </div>
                <div class="col-3">
                    <div class="ms-testimonial-card d-flex flex-column align-items-center">
                        <div class="ms-pp-container">
                            <img class="pp" src="../assets/img/testimonial-avata-01.jpg" alt="">
                        </div>
                        <p>MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                        <h5>MADLEY PONDOR</h5>
                        <small>/ IT Specialist</small>
                    </div>
                </div>
                <div class="col-3">
                    <div class="ms-testimonial-card d-flex flex-column align-items-center">
                        <div class="ms-pp-container">
                            <img class="pp" src="../assets/img/testimonial-avata-01.jpg" alt="">
                        </div>
                        <p>I am happy with their arrangement of lessons and subjects. They reflect a scienific innvestigation.</p>
                        <h5>LUVIC DUBBLE</h5>
                        <small>/ Private Tutor</small>
                    </div>
                </div>
            </div>
            <!-- Quattro puntini -->
            <div class="ms-dots d-flex justify-content-center">
                <ul class="d-flex justify-content-center align-items-center">
                    <li class="ms-first-dot d-flex"><i class="fa-solid fa-circle"></i></li>
                    <li><i class="fa-solid fa-circle"></i></li>
                    <li><i class="fa-solid fa-circle"></i></li>
                    <li><i class="fa-solid fa-circle"></i></li>
                </ul>
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

.ms-event-card{
    background-color: $light-gray;
    width: calc((100% / 2) - 20px);
    margin: 20px 10px;
    flex-wrap: wrap;
    padding: 15px 10px;
    border-radius: 5px;
    border-left: 2px solid transparent;

    &:hover{
        background-color: white;
        border-left: 2px solid $green;
        box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
        -webkit-box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
        -moz-box-shadow: 0px 14px 35px 33px rgba(0,0,0,0.05);
    }
    .ms-card-left{
        max-width: 50%;
        .ms-where{
            color: $gray;
        }
    }
    .ms-card-right{
        .ms-day{
            font-size: 45px;
            color: $green;
            font-weight: 100;
        }
        button{
            margin-top: 8px;
            background-color: $green;
            color: white;
            font-weight: 500;
            font-size: 14px;
            padding: 6px 18px;
            border: none;
            border-radius: 5px;
            &:hover{
            background-color: $purple;
        }
        }
    }
}
.events{
    a{
        text-decoration: none;
        color: $green;
    }
}


.testimonials{
    background-color: $light-gray;
    margin-top: 100px;
    .ms-testimonial-card{
         background-color: white;
         padding: 20px 0px;
         height: 325px;
         p{
            text-align: center;
            padding-top: 100px;
            padding-left: 15px;
            padding-right: 15px;
            padding-bottom: 20px;
         }
         small{
            font-size: 14px;
            font-weight: 200;
            color: $gray;
         }
    }

    .ms-pp-container{
        display: flex;
        position: relative;
        .pp{
            border-radius: 50%;
            position: absolute;
            width: 150px;
            top: -75px;
            right: -75px;
        }
    }
    .ms-dots{
        padding: 50px 0;
        ul{
            list-style: none;
            li{
                padding: 0 15px;
                color: $gray;
                font-size: 10px;
                font-weight: 100;
            }
            .ms-first-dot{
                font-size: 16px;
                font-weight: 600;
            }
        }
    }
}
</style>