<template>
    <div class="coverflow-example">
        <swiper class="swiper" :modules="[EffectCoverflow]" :pagination="true" :effect="'coverflow'" :grab-cursor="true"
            :centered-slides="true" :slides-per-view="'auto'" :coverflow-effect="{
                rotate: 50,
                stretch: 0,
                depth: 100,
                modifier: 1,
                slideShadows: true
            }">
            <swiper-slide class="slide" v-for="index in 8" :key="index">
                <img src="https://www.thewowstyle.com/wp-content/uploads/2015/01/nature-images.jpg" />
            </swiper-slide>
        </swiper>
    </div>
</template>

<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue'
import { EffectCoverflow } from 'swiper';

import 'swiper/css'
import 'swiper/css/effect-coverflow'

</script>

<style lang="scss" scoped>
.coverflow-example {
    position: relative;
}

.swiper {
    height: 100%;
    width: 100%;
    padding-top: 50px;
    padding-bottom: 50px;

    .slide {
        width: 300px;
        height: 300px;

        img {
            display: block;
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }
}
</style>