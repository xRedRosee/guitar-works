<template>
    <div class="loadingscreen" v-if="loading">
        <img src="../assets/gw-logo.png" alt="guitarworks logo" class="loading-img">
    </div>
</template>
<script>
export default {
    name: 'Loading',
    data() {
        return {
            loading: true,
        }
    },
    mounted() {
        this.loading = false
    }
}
</script>
<style scoped>
.loadingscreen {
    background-color: var(--white);
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: fixed;
    z-index: 9999;
    top: 0;
    opacity: 1;
}

.loading-img {
    height: 160px;
}

@media screen and (max-width: 680px) {
    .loading-img {
        height: 80px;
    }
}
</style>