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
                    target="_blank" class="facebook">
                    https://www.facebook.com/GuitarworksPanningen </a>
            </p>
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
}

.facebook:visited {
    color: black;
    font-weight: var(--normalfontmedium);
}
</style>