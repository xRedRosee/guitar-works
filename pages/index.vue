<template>
    <Navbar></Navbar>
    <section class="guitar-banner">
        <img src="../assets/banner.JPG" alt="guitar banner" class="banner-img">
        <span class="banner-overlay"></span>
        <h1 class="banner-text"> Guitarworks <br> Guitar Repair & Customizing Panningen</h1>
    </section>
</template>
<script>
import Navbar from '/././components/Navbar.vue';
export default {

}
</script>
<style>
.guitar-banner {
    height: 100vh;
    width: 100%;
    display: flex;
    flex-direction: column;
    position: relative;
    overflow: hidden;
    margin-top: -10px;
}

.banner-img {
    width: 100%;
}

.banner-overlay {
    position: absolute;
    top: 0;
    -webkit-box-shadow: inset 0px -22px 50px -5px rgba(0, 0, 0, 0.43);
    box-shadow: inset 0px -22px 50px -5px rgba(0, 0, 0, 0.43);
    width: 100%;
    height: 100%;
}

.banner-text {
    position: absolute;
    top: 50%;
    border-left: 8px solid var(--red);
    padding-left: 20px;
    font-size: 70px;
    color: var(--white);
    font-family: var(--headingfont);
    font-style: italic;
    font-weight: var(--headingfontweight);
    margin-left: 50px;
    text-shadow: 2px 2px 8px var(--black);
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 896px) {}

@media screen and (max-width: 768px) {
    .banner-img {
        height: 100%;
        margin-left: -689px;
    }
}
</style>