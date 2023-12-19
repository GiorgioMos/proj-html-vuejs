<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import { Pagination } from 'swiper/modules';

const pagination = {
    clickable: true,
    renderBullet: function (index, className) {
        return '<span class="' + className + '"></span>';
    },
};

const modules = [Pagination];
</script>

<template>
    <Swiper :pagination="pagination" :modules="modules" class="mySwiper">
        <SwiperSlide>
            <h2>High level of efficiency and scientific teaching methods</h2>
            <p>I am free to learn at my own pace, follow my own schedule and choose the subject i want</p>
            <div>
                <img src="../assets/img/testimonial-avata-02.jpg" alt="testimonial">
                <h5>MINA HOLLACE</h5>
                <p>/ Freelancer</p>
            </div>
        </SwiperSlide>
        <SwiperSlide>
            <h2>High level of efficiency and scientific teaching methods</h2>
            <p>I am free to learn at my own pace, follow my own schedule and choose the subject i want</p>
            <div>
                <img src="../assets/img/testimonial-avata-04.jpg" alt="testimonial">
                <h5>MADLEY PONDOR</h5>
                <p>/ IT specialist</p>
            </div>
        </SwiperSlide>
        <SwiperSlide>
            <h2>High level of efficiency and scientific teaching methods</h2>
            <p>I am free to learn at my own pace, follow my own schedule and choose the subject i want</p>
            <div>
                <img src="../assets/img/testimonial-avata-01.jpg" alt="testimonial">
                <h5>LUVIC DUBBLE</h5>
                <p>/ Private Tutor</p>
            </div>
        </SwiperSlide>
        <SwiperSlide>
            <h2>High level of efficiency and scientific teaching methods</h2>
            <p>I am free to learn at my own pace, follow my own schedule and choose the subject i want</p>
            <div class="card-container">
                <img src="../assets/img/testimonial-avata-03.jpg" alt="testimonial">
                <h5>FLORENCE THEMES</h5>
                <p>/ Multimedia Admin</p>
            </div>
        </SwiperSlide>
    </Swiper>
</template>

<style scoped lang="scss">
.mySwiper {
    width: 100%;
    height: 600px;
}

.swiper-slide {
    text-align: center;
    font-size: 18px;

    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.swiper-slide img {
    display: block;
    width: 70px;
    height: 70px;
    object-fit: cover;
    border-radius: 50%;
}

.swiper-pagination-bullet {
    width: 20px;
    height: 20px;
    background: rgba(0, 0, 0, 0.2);
}

.swiper-pagination-bullet-active {
    color: #20AD96;
}
</style>