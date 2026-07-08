<script setup>
const accessories = [
  {
    title: "Steam Deck",
    image: "images/steamdeck.jpg",
    link: "https://store.steampowered.com/steamdeck/"
  },
  {
    title: "Steam Gift Card",
    image: "images/giftcard.png",
    link: "https://store.steampowered.com/digitalgiftcards/"
  },
  {
    title: "Steam Controller",
    image: "images/controller.jpg",
    link: "https://store.steampowered.com/hardware/"
  }
]
</script>

<template>
<section class="accessories" id="accessories">

    <h2>アクセサリー</h2>

<a
    class="deck"
    :href="accessories[0].link"
    target="_blank"
    rel="noopener noreferrer"
>
    <img
        :src="accessories[0].image"
        :alt="accessories[0].title"
    >
</a>

    <div class="accessory-grid">

        <a
    class="accessory-card"
    v-for="item in accessories.slice(1)"
    :key="item.title"
    :href="item.link"
    target="_blank"
    rel="noopener noreferrer"
>

    <img :src="item.image" :alt="item.title">

    <h3>{{ item.title }}</h3>

</a>
    </div>

</section>
</template>

<style scoped>

</style>