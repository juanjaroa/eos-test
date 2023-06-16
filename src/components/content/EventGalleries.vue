
<template>
    <div id="gallery">
        <h2>Event Galleries</h2>

        <swiper :navigation="true" :modules="modules" class="card card-shadow mySwiper">
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

    </div>
</template>


<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/navigation';


// import required modules
import { Navigation } from 'swiper';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        return {
            modules: [Navigation],
        };
    },
};
</script>
<style scoped>
.swiper {
    width: 100%;
    height: 100%;
}

.swiper-slide {
    text-align: center;
    font-size: 18px;
    background: #fff;

    /* Center slide text vertically */
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

#gallery {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    align-items: stretch;
    height: 100%;
}

#gallery h2 {
    font-size: 1rem;
    font-weight: 300;
    text-align: center;
}

#gallery .card {
    background: #C4C4C4;
    padding: 0;
    height: 100%;
}

@media (min-width: 578px) {}

@media (min-width: 768px) {
    #gallery h2 {
        font-size: 2rem;
        font-weight: 500;
        text-align: left;
    }
}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>