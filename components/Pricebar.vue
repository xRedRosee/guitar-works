<template>
    <div class="pricebar">
        <p class="price-item"> {{ priceItem }}</p>
        <p class="price-number"> {{ priceNumber }}</p>
    </div>
</template>
<script>
export default {
    name: "Pricebar",
    props: {
        priceItem: String,
        priceNumber: String
    }
}
</script>
<style scoped>
.pricebar {
    background-color: var(--white);
    width: 95%;
    border-radius: 20px;
    height: 80px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding-inline: 19px;
    gap: 20px;
    -webkit-box-shadow: 0px 5px 14px -4px rgba(0, 0, 0, 0.27);
    box-shadow: 0px 5px 14px -4px rgba(0, 0, 0, 0.27);
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

.price-item {
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 20px;
    width: 85%;
}

.price-number {
    font-family: var(--normalfont);
    font-weight: var(--normalfontmedium);
    font-size: 20px;
    width: 15%;
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 1080px) {
    .pricebar {
        width: 90%;
    }
}

@media screen and (max-width: 680px) {
    .price-item {
        font-size: 18px;
        margin: 0;
        text-align: center;
        width: 90%;
    }

    .price-number {
        font-size: 18px;
        margin: 0;
        text-align: center;
        width: 80%;
    }

    .pricebar {
        height: 146px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 11px;
        box-shadow: 0px 5px 14px -4px rgba(0, 0, 0, 0.27);
        margin: 0;
        padding: 0;
    }
}
</style>