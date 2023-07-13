<template>
    <Navbar></Navbar>
    <section class="top-header">
        <Pagetitle pageTitle="Prijzen"></Pagetitle>
        <article class="header-intro-text">
            <p class="header-text"> Hieronder vindt u een aantal prijzen voor veel voorkomende werkzaamheden;
                voor een prijsopgave voor andere werkzaamheden kunt u vrijblijvend contact met ons opnemen via email
                <a href="mailto:guitarworks@live.nl" class="email"> guitarworks@live.nl</a> of per telefoon:
                <a href="tel:+31622209469" class="phone">06-22209469</a>
            </p>
            <div class="price-list">
                <Pricebar priceItem="Snaren vervangen inclusief reinigen en oliën van de toets: (exclusief snaren)"
                    priceNumber="€15,-"></Pricebar>
                <Pricebar priceItem="Lijmen gebroken hals" priceNumber="vanaf €30,-"></Pricebar>
                <Pricebar priceItem="Akoestische-, elektrische- of basgitaar (exclusief snaren)" priceNumber="€60,-">
                </Pricebar>
                <Pricebar priceItem="Vlakken en afstellen akoestische-, elektrische- of basgitaar (exclusief snaren)"
                    priceNumber="€90,-"></Pricebar>
                <Pricebar priceItem="Herfretten van gitaar met ongelakte toets (meestal Palissander)
zonder binding inclusief afstellen (exclusief snaren)" priceNumber="€200,-"></Pricebar>
                <Pricebar priceItem="Herfretten van gitaar met gelakte toets (meestal Esdoorn,
Palissander- of Ebben toets) met binding inclusief afstellen (exclusief snaren)
" priceNumber="€250,-">
                </Pricebar>
            </div>
            <p class="header-text warning-text"> Wij hebben <span class="bold">geen pin</span>; graag contante betaling bij
                ophalen van
                uw instrument! </p>
        </article>
    </section>
</template>
<script>
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
import Pricebar from '/././components/Pricebar.vue';
</script>
<style scoped>
.top-header {
    background-color: var(--lightgrey);
    padding-top: 20px;
    padding-bottom: 60px;
    -webkit-box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
    box-shadow: 0px 14px 22px -9px rgba(0, 0, 0, 0.1);
    overflow-x: hidden;
}

.header-intro-text {
    border-left: 5px solid var(--red);
    padding-left: 20px;
    margin-left: 20px;
}

.header-text {
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 20px;
    margin-block: 30px;
    width: 60%;
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

.price-list {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.bold {
    font-weight: var(--normalfontmedium);
}

.warning-text {
    width: 90%;
    text-align: center;
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 1080px) {
    .header-text {
        font-size: 18px;
        margin-block: 22px;
    }
}

@media screen and (max-width: 680px) {
    .header-text {
        font-size: 18px;
        margin-block: 22px;
        width: 90%;
    }

    .header-intro-text {
        width: 90%;
    }
}
</style>