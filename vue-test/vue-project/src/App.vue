<script setup>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import 'swiper/css';
</script>

<template>
    <h1>Параметры Видеокарт</h1>
    <div><img src="./img/cpu-svgrepo-com.svg" alt="cpu ico"> CPU: 0.2</div>
    <div><img src="./img/ram-memory-svgrepo-com.svg" alt="ram ico"> RAM: 7GB \ 62 GB</div>
    <div class="slider">
        <swiper
            :slides-per-view="1"
            :space-between="50"
            class="swiper"
        >
        <!-- первая видеокарта -->
            <swiper-slide>
                <div class="wrapper">
                    <h3 class="wrapper-header">Видеокарта 1</h3>
                    <div class="wrapper-properties">
                        <div class="means-name">
                            <span class="min">Минимальная: </span>
                            <span class="max">Максимальная: </span>
                            <span class="temp">Температура: </span>
                        </div>
                        <div class="means">
                            <span class="min-mean">0MiB</span>
                            <span class="max-mean">6144MiB</span>
                            <span class="temp-mean">54С</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <!-- Вторая видеокарта -->
            <swiper-slide>
                <div class="wrapper">
                    <h3 class="wrapper-header">Видеокарта 2</h3>
                    <div class="wrapper-properties">
                        <div class="means-name">
                            <span class="min">Минимальная: </span>
                            <span class="max">Максимальная: </span>
                            <span class="temp">Температура: </span>
                        </div>
                        <div class="means">
                            <span class="min-mean">0MiB</span>
                            <span class="max-mean">6144MiB</span>
                            <span class="temp-mean">54С</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <!-- Третья видеокарта -->
            <swiper-slide>
                <div class="wrapper">
                    <h3 class="wrapper-header">Видеокарта 3</h3>
                    <div class="wrapper-properties">
                        <div class="means-name">
                            <span class="min">Минимальная: </span>
                            <span class="max">Максимальная: </span>
                            <span class="temp">Температура: </span>
                        </div>
                        <div class="means">
                            <span class="min-mean">0MiB</span>
                            <span class="max-mean">6144MiB</span>
                            <span class="temp-mean">54С</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
        </swiper>
    </div>
</template>

<style scoped>
    .wrapper {
    background-color: black;
    border-radius: 10px;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
}

.wrapper > * {
    color: white;
}

.wrapper-header {
    padding: 20px 10px;
}

.wrapper-properties {
    display: flex;
    flex-wrap: wrap;
    padding-left: 10px;
    justify-content: space-between;
}

.wrapper-properties > * {
    margin: 6px;
}

.means-name {
    display: flex;
    flex-direction: column;
}

.means-name > * {
    margin-top: 6px;
}

.means {
    color: orange;
    display: flex;
    flex-direction: column;
}

.means > * {
    margin-top: 7px;
}

.slider {
    padding: 50px 0
}
.swiper {
    width: 400px;
}
</style>
