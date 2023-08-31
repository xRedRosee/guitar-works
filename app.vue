<template>
  <Head>
    <Title>Guitarworks</Title>
    <Meta name="guitarworks" content="Guitarworks" />
  </Head>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
  <Copyright></Copyright>
</template>
<script setup>
import Copyright from '/././components/Copyright.vue';
</script>
<style>
@import url("https://use.typekit.net/psc6wfy.css");

:root {
  --black: black;
  --white: white;
  --red: #C00808;
  --lightgrey: #F1F1F1;
  --normalfont: "canada-type-gibson", sans-serif;
  --normalfontnormal: 400;
  --normalfontmedium: 500;
  --normalfontbold: 700;
  --headingfont: "lorimer-no-2", sans-serif;
  --headingweight: 700;
  --headingstyle: italic;
}

body {
  margin: 0;
  padding: 0;
}
</style>
