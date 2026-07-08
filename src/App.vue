<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import AboutSteam from './components/AboutSteam.vue'
import GameList from './components/GameList.vue'
import Accessories from './components/Accessories.vue'
import Community from './components/Community.vue'
import Support from './components/Support.vue' 
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />
  <Hero />
  <AboutSteam />
  <GameList />
  <Accessories />

  <hr class="divider">

  <Community />

  <hr class="divider">

  <Support />

  <Footer />
</template>