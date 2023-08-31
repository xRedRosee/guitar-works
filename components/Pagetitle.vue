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
    animation: 0.5s ease-out fadeIn;
}

@keyframes fadeIn {
    0% {
        opacity: 0;
        margin-left: -100px;
    }

    100% {
        opacity: 1;
        margin-left: 40px;
    }
}

@-webkit-keyframes fadeIn {
    0% {
        opacity: 0;
        margin-left: -100px;
    }

    100% {
        opacity: 1;
        margin-left: 40px;
    }
}

@media screen and (max-width: 680px) {
    .header-h1 {
        font-size: 40px;
    }
}
</style>