<template>
    <Loading></Loading>
    <Navbar></Navbar>
    <section class="top-header">
        <Pagetitle pageTitle="Pedalboards"></Pagetitle>
        <div class="header-info">
            <div class="text-side">
                <article class="header-intro-text">
                    <p class="header-text">Als gitarist zijnde begeef je je vroeg of laat in de wereld van gitaareffecten.
                        Naarmate dat de hoeveelheid effecten (meestal in pedaalvorm) zich uitbreiden, ontstaan ook de eerste
                        problemen.
                    </p>
                    <p class="header-text"> - Welke volgorde van effecten moet ik hanteren? <br>
                        - Wat voor patch (verbindings) kabeltjes kan ik het beste gebruiken? <br>
                        - Welke voeding kan ik het beste gebruiken? <br>
                        Ik wil alles graag idiot proof een road-ready gemonteerd hebben… Kan dat?
                    </p>
                    <p class="header-text"> Ja, wij bij Guitarworks hebben al bijna 100 pedalboard gebouwd om er voor te
                        zorgen dat zowel de hobby-gitarist alsook de professionele-gitarist probleemloos met zijn
                        ‘’effectenbundel’’ kan spelen zonder last te hebben van ruis-, brom-, kabel- of voedingsproblemen.
                        Wij maken een pedalboard op maat met desgewenst ook een multisnake (=kabelbundel) op maat.
                    </p>
                </article>
            </div>
            <div class="img-side">
                <img class="header-img" alt="pedalboard foto" src="../assets/pedalboards.JPG">
            </div>
        </div>
    </section>
    <section class="beeld-section">
        <Pagetitle pageTitle="Pedalboards in beeld"></Pagetitle>
        <p class="beeld-intro"> Deze foto’s geven je een impressie van wat er mogelijk is… </p>
        <div class="glide slide-div beeld-slides">
            <div class="glide__track" data-glide-el="track">
                <ul class="glide__slides">
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard1.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard2.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard3.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard4.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard5.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard6.jpeg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard7.jpeg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard8.jpeg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/pedalboard9.jpg" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/Multi-Snake-op-maat.jpg" alt="pedal board" class="show-img">
                    </li>
                </ul>
            </div>
            <div class="glide__controls buttons" data-glide-el="controls">
                <button class="glide__arrow glide__arrow--left button-left" data-glide-dir="|<">
                    <img alt="arrow left" class="arrow-img" src="../assets/arrow-left-red.svg">
                </button>
                <button class="glide__arrow glide__arrow--right button-right" data-glide-dir="|>">
                    <img alt="arrow right" class="arrow-img" src="../assets/arrow-right-red.svg">
                </button>
            </div>
        </div>
    </section>
</template>
<script>
import Glide from '@glidejs/glide'
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
import { reloadNuxtApp } from 'nuxt/app';
import Loading from '/././components/Loading.vue';

export default {
    mounted() {
        reloadNuxtApp();
        new Glide('.glide', {
            type: 'carousel',
            animationDuration: 2000,
            // go to next slide after 7 seconds
            autoplay: 7000,
            // show 1 slide, starting with first slide
            focusAt: '1',
            startAt: 1,
            perView: 1,
            gap: 0,
        }).mount()
    },
}
</script>
<style scoped>
@import '@glidejs/glide/dist/css/glide.core.min.css';

.top-header {
    background-color: var(--lightgrey);
    padding-top: 20px;
    padding-bottom: 60px;
    -webkit-box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
    box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
}

.header-info {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.text-side {
    width: 50%;
}

.header-intro-text {
    width: 80%;
    border-left: 5px solid var(--red);
    padding-left: 20px;
    margin-left: 20px;
}

.header-text {
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 20px;
    margin-block: 30px;
    animation: 1s ease-out opacityChange;
}

@keyframes opacityChange {
    0% {
        opacity: 0;
    }

    100% {
        opacity: 1;
    }
}

@-webkit-keyframes opacityChange {
    0% {
        opacity: 0;
    }

    100% {
        opacity: 1;
    }
}

.img-side {
    width: 50%;
    display: flex;
    justify-content: center;
}

.header-img {
    width: 60%;
    animation: 0.5s ease-out slideInRight;
}

@keyframes slideInRight {
    0% {
        opacity: 0;
        margin-right: -100px;
    }

    100% {
        opacity: 1;
        margin-right: 0;
    }
}

@-webkit-keyframes slideInRight {
    0% {
        opacity: 0;
        margin-right: -100px;
    }

    100% {
        opacity: 1;
        margin-right: 0;
    }
}

.beeld-section {
    margin-top: 20px;
}

.beeld-intro {
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 20px;
    margin: 0;
    margin-left: 40px;
    margin-top: 20px;
}

.beeld-slides {
    margin-top: 40px;
    margin-bottom: 30px;
    position: relative;
    display: flex;
    justify-content: center;
}

.show-slide {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.show-img {
    height: 300px;
}

.buttons {
    position: absolute;
    top: 50%;
    display: flex;
    flex-direction: row;
    width: 90%;
    justify-content: space-between;
}

.button-left {
    margin: 0;
    /* margin-left: 90px; */
    font-size: 30px;
    background: none;
    /* color: var(--red); */
    outline: none;
    /* border: solid 2px var(--red); */
    border-radius: 50%;
    padding: 0;
    height: 60px;
    width: 60px;
    cursor: pointer;
    border: none;
    display: flex;
    justify-content: center;
    align-items: center;
}

.button-right {
    margin: 0;
    /* margin-right: 90px; */
    font-size: 30px;
    background: none;
    /* color: var(--red); */
    outline: none;
    /* border: solid 2px var(--red); */
    border-radius: 50%;
    padding: 0;
    height: 60px;
    width: 60px;
    cursor: pointer;
    border: none;
    display: flex;
    justify-content: center;
    align-items: center;
}

.arrow-img {
    height: 70px;
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 1080px) {
    .header-img {
        width: 80%;
    }

    .header-intro-text {
        width: 90%;
    }

    .header-text {
        font-size: 18px;
        margin-block: 22px;
    }

    .beeld-intro {
        font-size: 18px;
    }

    .show-img {
        width: 70%;
        height: auto;
    }

    .buttons {
        bottom: 0%;
        top: auto;
    }

    .show-slide {
        padding-bottom: 34px;
    }

    .glide__slides {
        display: flex;
        justify-content: center;
        align-items: center;
    }

}

@media screen and (max-width: 680px) {
    .header-info {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
    }

    .text-side {
        display: flex;
        width: 90%;
        justify-content: center;
        margin-bottom: 20px;
    }

    .header-intro-text {
        width: 100%;
        margin-left: 0;
        border-left: 4px solid var(--red);
    }

    .img-side {
        width: 90%;
        display: flex;
        justify-content: center;
    }

    .header-text {
        font-size: 18px;
        margin-block: 22px;
    }

    .show-img {
        width: 90%;
        height: auto;
    }

    .show-slide {
        padding-bottom: 73px;
    }

    .glide__slides {
        justify-content: center;
        align-items: center;
    }
}
</style>