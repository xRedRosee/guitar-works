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
</style>