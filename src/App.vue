<script setup lang="ts">
import { RouterView } from "vue-router";
import Header from './components/Header.vue';
import AppWelcome from './components/AppWelcome.vue';
import Footer from './components/Footer.vue';
import Spacer from './components/Spacer.vue';
</script>

<template>
  <header>
  </header>
  <main id="appContainer">
    <Header msg="Wholemart" />
    <RouterView />
    <Spacer />
    <Footer />
  </main>
</template>

<style scoped>
  #appContainer {
    display: flex;
    height: 100vh;
    flex-direction: column;
  }
</style>
