
<template>
    <div id="gallery">
        <h2>Event Galleries</h2>

        <swiper @swiper="onSwiper" :navigation="false" :loop="true" :autoplay="{
            delay: 3500,
        }" :modules="modules" class="card card-shadow mySwiper">

            <swiper-slide v-for="(index) in 10" :key="index" class="swiper"
                :style="{ background: 'url(' + backGround + index + ')', backgroundSize: 'cover', backgroundPosition: 'center' }">
                <div class="control">
                    <button @click.stop="slider.slidePrev()"><img src="./assets/left.png" alt=""></button>
                    <span>SLIDE {{ index }}</span>
                    <button @click.stop="slider.slideNext()"><img src="./assets/right.png" alt=""></button>
                </div>
            </swiper-slide>
        </swiper>

    </div>
</template>


<script>
// Import Swiper Vue.js components
import { ref } from "vue";
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/navigation';


// import required modules
import { Autoplay, Navigation } from 'swiper';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        const slider = ref(null)
        const onSwiper = (swiper) => {
            slider.value = swiper;
        };
        return {
            modules: [Autoplay, Navigation],
            backGround: 'https://picsum.photos/800/600?random=',
            slider,
            onSwiper
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
    display: flex;
    justify-content: center;
    align-items: center;
}


.control {
    position: absolute;
    bottom: 1rem;
    display: flex;
    width: 90%;
    justify-content: space-between;
    align-items: center;
}

.control img,
.control span {
    filter: drop-shadow(0 0 5px rgba(0, 0, 0, 0.2));
}

button {
    background: transparent;
    cursor: pointer;
}

button img {
    width: 0.75rem;
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

@media (min-width: 992px) {
    .control {
        width: 60%;
    }
}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>