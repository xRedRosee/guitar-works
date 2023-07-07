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
</template>
<script>
import Navbar from '/././components/Navbar.vue';
import Pagetitle from '/././components/Pagetitle.vue';
export default {

}
</script>
<style scoped>
.top-header {
    background-color: var(--lightgrey);
    padding-top: 20px;
    padding-bottom: 60px;
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