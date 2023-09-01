<template>
    <div class="bar">
        <p class="copyright-text"> Copyright © 2023 Designed by Iris Roemermann</p>
    </div>
</template>
<script>
export default {
    name: "Copyright",
}
</script>
<style>
.bar {
    width: 100%;
    background-color: black;
    padding: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 25px;
    margin: 0;
}

.copyright-text {
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 100;
}
</style>