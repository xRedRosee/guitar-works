<template>
    <h1 class="header-h1"> {{ pageTitle }}</h1>
</template>
<script>
export default {
    name: "Pagetitle",
    props: {
        pageTitle: String
    }
}
</script>
<style scoped>
.header-h1 {
    font-size: 50px;
    color: var(--black);
    font-family: var(--headingfont);
    font-style: italic;
    font-weight: var(--headingfontweight);
    margin: 0;
    margin-left: 40px;
}

@media screen and (max-width: 680px) {
    .header-h1 {
        font-size: 40px;
    }
}
</style>