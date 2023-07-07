<template>
    <div class="pricebar">
        <p> {{ priceItem }}</p>
        <p> {{ priceNumber }}</p>
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
}
</style>