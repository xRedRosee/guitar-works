<template>
    <Loading></Loading>
    <Navbar></Navbar>
    <section class="top-header">
        <Pagetitle pageTitle="Contact"></Pagetitle>
        <article class="header-intro-text">
            <p class="header-text"> Wij zijn bereikbaar via email: <a href="mailto:guitarworks@live.nl" class="email">
                    guitarworks@live.nl</a> of per telefoon:
                <a href="tel:+31622209469" class="phone">06-22209469</a>
            </p>
            <p class="header-text">
                Verder zijn wij te vinden op Facebook: <a href="https://www.facebook.com/GuitarworksPanningen"
                    target="_blank" class="facebook"> www.facebook.com/GuitarworksPanningen </a>
            </p>
            <section class="contact-info">
                <article class="adress-section">
                    <h1 class="contact-header"> Adres </h1>
                    <p class="contact-text"> Guitarworks </p>
                    <p class="contact-text"> Burg. Janssenring 32 </p>
                    <p class="contact-text"> 5981 DH Panningen</p>
                </article>
                <article class="tijd-section">
                    <h1 class="contact-header"> Openingstijden op afspraak </h1>
                    <p class="contact-text"> Maandag tot vrijdag </p>
                    <p class="contact-text"> Tussen 10:00 tot 17:00 </p>
                </article>
            </section>
        </article>
        <a href="https://goo.gl/maps/CaK8b7hmsjir1UGq5" class="map-link" target="_blank">
            <img src="../assets/Guitarworks-map.jpg" alt="guitarworks map" class="map-img">
        </a>
    </section>
</template>
<script>
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
import Loading from '/././components/Loading.vue';

export default {

}
</script>
<style scoped>
.top-header {
    background-color: var(--lightgrey);
    padding-top: 20px;
    padding-bottom: 60px;
    -webkit-box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
    box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
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

.email {
    color: black;
    font-weight: var(--normalfontmedium);
}

.email:visited {
    color: black;
    font-weight: var(--normalfontmedium);
}

.phone {
    color: black;
    font-weight: var(--normalfontmedium);
}

.phone:visited {
    color: black;
    font-weight: var(--normalfontmedium);
}

.facebook {
    color: black;
    font-weight: var(--normalfontmedium);
    word-wrap: break-word;
}

.facebook:visited {
    color: black;
    font-weight: var(--normalfontmedium);
}

.contact-info {
    display: flex;
    justify-content: space-between;
    width: 90%;
}

.adress-section {
    width: 50%;
    animation: 0.5s ease-out slide;
}

@keyframes slide {
    0% {
        opacity: 0;
        margin-left: -50px;
    }

    100% {
        opacity: 1;
        margin-left: 0;
    }
}

@-webkit-keyframes slide {
    0% {
        opacity: 0;
        margin-left: -50px;
    }

    100% {
        opacity: 1;
        margin-left: 0;
    }
}

.contact-header {
    color: black;
    font-weight: var(--normalfontmedium);
    font-family: var(--normalfont);
    font-size: 24px;
    margin-bottom: 20px;
}

.contact-text {
    color: black;
    font-family: var(--normalfont);
    font-size: 20px;
    margin-block: 10px;
}

.tijd-section {
    width: 50%;
    animation: 0.5s ease-out slideIn;
}

@keyframes slideIn {
    0% {
        opacity: 0;
        margin-right: -50px;
    }

    100% {
        opacity: 1;
        margin-right: 0;
    }
}

@-webkit-keyframes slideIn {
    0% {
        opacity: 0;
        margin-right: -50px;
    }

    100% {
        opacity: 1;
        margin-right: 0;
    }
}

.map-link {
    width: 100%;
    display: flex;
    justify-content: center;
}

.map-img {
    margin-top: 60px;
    width: 65%;
}

@media screen and (max-width: 1080px) {
    .header-intro-text {
        width: 90%;
    }

    .map-img {
        width: 80%;
    }
}

@media screen and (max-width: 680px) {
    .contact-info {
        display: flex;
        justify-content: space-between;
        width: 90%;
        flex-direction: column;
    }

    .adress-section {
        width: 100%;
    }

    .tijd-section {
        width: 100%;
    }

    .map-img {
        width: 90%;
    }
}
</style>