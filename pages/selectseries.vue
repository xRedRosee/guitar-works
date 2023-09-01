<template>
    <Navbar></Navbar>
    <section class="top-header">
        <Pagetitle pageTitle="Select Series"></Pagetitle>
        <div class="header-info">
            <div class="text-side">
                <article class="header-intro-text">
                    <p class="header-text">Het Select Series verhaal is een concept dat we bedacht hebben om iedere gitarist
                        met een minimaal budget van €500,- te kunnen helpen aan de gitaar die voldoet aan de wensen van de
                        gitarist. </p>
                    <p class="header-text"> Om deze gitaar te kunnen samenstellen maken we gebruik van nieuwe en gebruikte
                        onderdelen. Op deze manier kunnen we toch met een kleiner budget een coole en unieke gitaar
                        samenstellen
                    </p>
                    <p class="header-text"> Dus kom met je wensenlijst en budget naar ons toe en wij kijken hoe we je droom
                        gitaar kunnen verwezenlijken!
                    </p>
                    <p class="header-text"> We hebben er inmiddels al bija 60 gemaakt in prijsklassen variërend van €500,-
                        tot ca €2000,-
                    </p>
                </article>
            </div>
            <div class="img-side">
                <img class="header-img" alt="select series foto" src="../assets/SelectSeries/SelectSeriesparts.jpg">
            </div>
        </div>
    </section>
    <section class="beeld-section">
        <Pagetitle pageTitle="Select Series in beeld"></Pagetitle>
        <p class="beeld-intro"> Deze foto’s geven je een impressie van wat er mogelijk is… </p>
        <div class="glide slide-div beeld-slides">
            <div class="glide__track" data-glide-el="track">
                <ul class="glide__slides">
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries11.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries14.jpg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries33.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries35.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries42.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries46.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries47.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries48.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries49.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries51-2.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries52.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries53.jpg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries54.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries55.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries57.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeries58.jpeg" alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeriesPrivatCollectionCoronaGreen.jpeg"
                            alt="select series guitar" class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/SelectSeriesProto.jpeg" alt="select series guitar"
                            class="show-img">
                    </li>
                    <li class="glide__slide show-slide">
                        <img src="../assets/SelectSeries/Select-Series-5.jpeg" alt="select series guitar" class="show-img">
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
import Glide from '@glidejs/glide';
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
export default {
    beforeMount() {
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