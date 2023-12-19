<script setup>
import { RouterView } from "vue-router"
import Header from "./components/Header.vue"
import FooterVue from "./components/Footer.vue"
</script>

<template>
  <Header />
  <RouterView />
  <FooterVue />
</template>
