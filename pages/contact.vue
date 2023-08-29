<template>
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
    </section>
</template>
<script>
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
export default {

}
</script>
<style>
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
}

@media screen and (max-width: 1080px) {
    .header-intro-text {
        width: 90%;
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
}
</style>