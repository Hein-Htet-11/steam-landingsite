<script setup>
const games = [
  {
    category: "新作ゲーム",
    title: "Red Dead Redemption II",
    image: "images/rdr2.jpg",
    link: "https://store.steampowered.com/app/1174180/Red_Dead_Redemption_2/"
  },
  {
    category: "人気ゲーム",
    title: "Cyberpunk 2077",
    image: "images/cyberpunk.jpg",
    link: "https://store.steampowered.com/app/1091500/Cyberpunk_2077/"
  },
  {
    category: "RPG",
    title: "Like a Dragon: Infinite Wealth",
    image: "images/yakuza.jpg",
    link: "https://store.steampowered.com/app/2072450/Like_a_Dragon_Infinite_Wealth/"
  },
  {
    category: "アクションゲーム",
    title: "Assassin's Creed Shadows",
    image: "images/ac.jpg",
    link: "https://store.steampowered.com/app/3159330/Assassins_Creed_Shadows/"
  }
]
</script>

<template>

<section class="games" id="games">

    <h2>ゲーム一覧</h2>

    <div class="game-grid">

<a
  class="game-card"
  v-for="game in games"
  :key="game.title"
  :href="game.link"
  target="_blank"
  rel="noopener noreferrer"
>

    <img :src="game.image" :alt="game.title">

    <h4>{{ game.category }}</h4>

    <h3>{{ game.title }}</h3>

</a>

    </div>

</section>

</template>

<style scoped>

</style>