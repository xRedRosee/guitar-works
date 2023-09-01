<template>
    <Navbar></Navbar>
    <section class="guitar-banner">
        <div class="guitar-img">
            <img src="../assets/banner2.jpg" alt="guitar banner" class="banner-img">
            <img src="../assets/banner.jpg" alt="guitar banner" class="banner-img-small">
            <div class="line"></div>
            <h1 class="banner-text"> Guitarworks <br> Guitar Repair & Customizing Panningen</h1>
        </div>
    </section>
</template>
<script>
import Navbar from '/././components/Navbar.vue';
export default {

}
</script>
<style scoped>
.guitar-banner {
    height: 100vh;
    width: 100%;
    overflow: hidden;
}

.guitar-img {
    position: relative;
    overflow: hidden;
    /* height: 115%; */
}

.banner-img {
    width: 100%;
    height: auto;
    /* height: 100%; */
    margin-top: 20px;
}

.banner-img-small {
    margin: 0;
    height: 100%;
    width: auto;
    transform: rotate(270deg);
    margin-top: 20px;
    display: none;
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
    margin-block: 0;
    animation: 0.5s ease-out slideDown;
}

@keyframes slideDown {
    0% {
        margin-top: -100px;
        opacity: 0;
    }

    100% {
        margin-top: 0;
        opacity: 1;
    }
}

@-webkit-keyframes slideDown {
    0% {
        margin-top: -100px;
        opacity: 0;
    }

    100% {
        margin-top: 0;
        opacity: 1;
    }
}

.line {
    position: absolute;
    height: 8px;
    background-color: var(--red);
    width: 40%;
    top: 5%;
    right: 30px
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 1010px) {
    /* .guitar-img {
        height: 100%;
    }

    .banner-img {
        height: 100%;
        width: auto;
        margin-left: -168px;
    }

    .banner-text {
        position: absolute;
        top: 50%;
        font-size: 50px;
    } */

    .guitar-img {
        position: relative;
        overflow: hidden;
        height: 100%;
    }

    .banner-img {
        display: none;
    }

    .banner-img-small {
        display: block;
    }

    .banner-text {
        position: absolute;
        top: 70%;
        font-size: 50px;
        margin-left: 21px;
    }

    .guitar-img {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .line {
        display: none;
    }
}

@media screen and (max-width: 768px) {
    .banner-img {
        display: none;
    }

    .banner-img-small {
        display: block;
    }

    .banner-text {
        position: absolute;
        top: 70%;
        font-size: 50px;
        margin-left: 21px;
    }

    .guitar-img {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .line {
        display: none;
    }
}

@media screen and (max-width: 550px) {
    .banner-text {
        position: absolute;
        top: 50%;
        font-size: 30px;
        margin-left: 21px;
    }
}

/*

@media screen and (max-width: 420px) {
    .banner-img {
        height: 100%;
        margin-left: -729px;
    }
}

@media screen and (max-width: 380px) {
    .banner-img {
        height: 100%;
        margin-left: -571px;
    }
}

@media screen and (max-height: 550px) {
    .banner-img {
        width: 100%;
        height: auto;
        margin-left: 0;
    }

    .banner-text {
        position: absolute;
        top: 30%;
        font-size: 50px;
    }
} */
</style>