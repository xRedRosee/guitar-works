<template>
    <Navbar></Navbar>
    <section class="top-header">
        <Pagetitle pageTitle="Ons werk"></Pagetitle>
        <div class="header-info">
            <div class="text-side">
                <article class="header-intro-text">
                    <p class="header-text"> Bij Guitarworks houden we ons bezig met de meest voorkomende reparatie- en
                        afstelwerkzaamheden aan gitaren en aanverwanten.</p>
                    <p class="header-text">Wij verbeteren de bespeelbaarheid van uw instrument, verhelpen eventuele
                        storingen aan de electronica of customizen het instrument naar uw wensen.</p>
                    <p class="header-text"> Schade aan lak of hout van de gitaar? Ook hiervoor kunt u bij ons terecht. Kom
                        bij voorkeur een keer langs voor een juiste prijsopgave… </p>
                    <p class="header-text"> Daarnaast kunnen wij onder de noemer Select Series een gitaar voor u
                        samenstellen die voldoet aan uw wensen… Prijzen op aanvraag…</p>
                    <p class="header-text">Pedalboard problemen? Ook die lossen we voor u op! Dit kan zijn bij uw bestaande
                        pedalboard of we maken een compleet nieuw custom pedalboard. Prijzen op aanvraag…</p>
                </article>
            </div>
            <div class="img-side">
                <img class="header-img" alt="over ons foto" src="../assets/onswerk-img.jpg">
            </div>
        </div>
    </section>
    <section class="beeld-section">
        <Pagetitle pageTitle="Ons werk in beeld"></Pagetitle>
        <div class="glide slide-div beeld-slides">
            <div class="glide__track" data-glide-el="track">
                <ul class="glide__slides">
                    <li class="glide__slide show-slide">
                        <img alt="werk in beeld foto" class="show-img"
                            src="../assets/Onswerk/Afstellen en intoneren van een basgitaar....JPG">
                        <p class="show-text">Afstellen en intoneren van een basgitaar </p>
                    </li>
                    <li class="glide__slide show-slide">
                        <img alt="werk in beeld foto" class="show-img"
                            src="../assets/Onswerk/Brug lijmen van western gitaar... (m.b.v. onze specialisten...).JPG">
                        <p class="show-text">Brug lijmen van western gitaar (m.b.v. onze specialisten) </p>
                    </li>
                    <li class="glide__slide show-slide">
                        <img alt="werk in beeld foto" class="show-img"
                            src="../assets/Onswerk/Custom schakelingen in de electronica aanbrengen....JPG">
                        <p class="show-text">Custom schakelingen in de electronica aanbrengen </p>
                    </li>
                </ul>
            </div>
            <div class="glide__controls buttons" data-glide-el="controls">
                <button class="glide__arrow glide__arrow--left button-left" data-glide-dir="|<">&#8592;</button>
                <button class="glide__arrow glide__arrow--right button-right" data-glide-dir="|>">&#8594;</button>
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
}

.img-side {
    width: 50%;
    display: flex;
    justify-content: center;
}

.header-img {
    width: 65%;
}

.beeld-section {
    margin-top: 20px;
}

.beeld-slides {
    margin-top: 40px;
    margin-bottom: 30px;
    position: relative;
}

.show-slide {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.show-img {
    height: 350px;
}

.show-text {
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 20px;
    margin-block: 30px;
}

.buttons {
    position: absolute;
    top: 50%;
    display: flex;
    flex-direction: row;
    width: 100%;
    justify-content: space-between;
}

.button-left {
    margin-left: 90px;
    font-size: 30px;
    background: none;
    color: var(--red);
    outline: none;
    border: solid 2px var(--red);
    border-radius: 50%;
    padding: 0;
    height: 60px;
    width: 60px;
    cursor: pointer;
}

.button-right {
    margin-right: 90px;
    font-size: 30px;
    background: none;
    color: var(--red);
    outline: none;
    border: solid 2px var(--red);
    border-radius: 50%;
    padding: 0;
    height: 60px;
    width: 60px;
    cursor: pointer;
}


/* -------------------------------------------- media queries */
@media screen and (max-width: 1080px) {
    .header-img {
        width: 85%;
    }

    .header-intro-text {
        width: 90%;
    }

    .header-text {
        font-size: 18px;
        margin-block: 22px;
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
}
</style>