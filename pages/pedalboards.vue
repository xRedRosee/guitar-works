<template>
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
                        <img src="../assets/Pedalboards/pedalboard9.JPG" alt="pedal board" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/Pedalboards/Multi Snake op maat....JPG" alt="pedal board" class="show-img">
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
export default {
    mounted() {
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
<style>
@import '@glidejs/glide/dist/css/glide.core.min.css';
</style>