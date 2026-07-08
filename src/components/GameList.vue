<script setup>
const games = [
  {
    category: "新作ゲーム",
    title: "Red Dead Redemption II",
    image: "images/rdr2.jpg"
  },
  {
    category: "人気ゲーム",
    title: "Cyberpunk 2077",
    image: "images/cyberpunk.jpg"
  },
  {
    category: "RPG",
    title: "Like a Dragon: Infinite Wealth",
    image: "images/yakuza.jpg"
  },
  {
    category: "アクションゲーム",
    title: "Assassin's Creed Shadows",
    image: "images/ac.jpg"
  }
]
</script>

<template>

<section class="games" id="games">

    <h2>ゲーム一覧</h2>

    <div class="game-grid">

        <div
  class="game-card"
  v-for="game in games"
  :key="game.title"
>
    <img :src="game.image" :alt="game.title">

    <h4>{{ game.category }}</h4>

    <h3>{{ game.title }}</h3>

</div>

    </div>

</section>

</template>

<style scoped>

</style>