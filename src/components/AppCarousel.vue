<script setup>
import 'swiper/css'; // Import Swiper styles
import 'swiper/css/pagination';
import Swiper, { Pagination } from 'swiper'; // Import Swiper core and required modules

const pagination = {
    clickable: true,
};

const modules = [Pagination];

// Initialize Swiper when the component is mounted
onMounted(() => {
    const mySwiper = new Swiper('.mySwiper', {
        pagination,
        modules,
    });
});

// Destroy Swiper instance when the component is unmounted
onUnmounted(() => {
    const mySwiper = document.querySelector('.mySwiper');
    if (mySwiper && mySwiper.swiper) {
        mySwiper.swiper.destroy();
    }
});
</script>

<template>
    <swiper class="mySwiper">
        <swiper-slide>Slide 1</swiper-slide>
        <swiper-slide>Slide 2</swiper-slide>
        <swiper-slide>Slide 3</swiper-slide>
        <swiper-slide>Slide 4</swiper-slide>
        <swiper-slide>Slide 5</swiper-slide>
        <swiper-slide>Slide 6</swiper-slide>
        <swiper-slide>Slide 7</swiper-slide>
        <swiper-slide>Slide 8</swiper-slide>
        <swiper-slide>Slide 9</swiper-slide>
    </swiper>
</template>

<style scoped lang="scss">
.mySwiper {
    width: 100%;
    height: 100%;
}

.swiper-slide {
    text-align: center;
    font-size: 18px;
    background: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
}

.swiper-slide img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.swiper-pagination-bullet {
    width: 20px;
    height: 20px;
    background: rgba(0, 0, 0, 0.2);
}

.swiper-pagination-bullet-active {
    background: #007aff;
}
</style>
