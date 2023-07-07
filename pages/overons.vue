<template>
    <Navbar></Navbar>
    <section class="top-header">
        <h1 class="header-h1"> Over ons </h1>
        <div class="header-info">
            <div class="text-side">
                <article class="header-intro-text">
                    <p class="header-text"> Guitarworks is een eenmanszaak, in 2008 opgericht door Dick Roemermann. Met 25
                        jaar
                        ervaring binnen de gitaarbranche, heeft Dick inmiddels zijn sporen verdiend. </p>
                    <p class="header-text"> Na afronding van zijn studie gitaarbouw in 1999 is Dick van 1999-2008 werkzaam
                        geweest bij Muziekcentrum Reijnen Roermond. Hierna werkte hij 2 jaar als afdelingshoofd bij Muzikaza
                        Reijnen Roermond.</p>
                    <p class="header-text"> Tussen 2010-2012 is Dick betrokken geweest bij GearPro in Nederweert. Enkele
                        ontwikkelingen hebben hem uiteindelijk doen besluiten om per 1 januari 2013 volledig zelfstandig en
                        fulltime met Guitarworks in Panningen verder te gaan. </p>
                </article>
            </div>
            <div class="img-side">
                <img class="header-img" alt="over ons foto" src="../assets/IMG_5953.jpeg">
            </div>
        </div>
    </section>
    <article class="bottom-banner">
        <p class="bottom-text">Guitarworks is hét Gitaar Repair en Customizing Center van Limburg. Alles wat het fenomeen
            “gitaar” ademt is welkom.
            Of het nu gaat om eenvoudig vervangen van snaren, het repareren van schade of het laten bouwen van een ‘’Select
            Series Gitaar’’ of pedalboard: Guitarworks is voor dit alles het juiste adres.</p>
    </article>
</template>
<script scoped>
import Navbar from '/././components/Navbar.vue';
export default {

}
</script>
<style>
.top-header {
    background-color: var(--lightgrey);
    padding-top: 20px;
    padding-bottom: 60px;
}

.header-h1 {
    font-size: 50px;
    color: var(--black);
    font-family: var(--headingfont);
    font-style: italic;
    font-weight: var(--headingfontweight);
    margin: 0;
    margin-left: 40px;
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
    width: 60%;
}

.bottom-banner {
    width: 100%;
    display: flex;
    justify-content: center;
    padding-block: 50px;
}

.bottom-text {
    font-family: var(--normalfont);
    font-weight: var(--normalfontmedium);
    font-size: 22px;
    width: 80%;
    text-align: center;
}
</style>