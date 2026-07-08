<script setup>
const accessories = [
  {
    title: "Steam Deck",
    image: "images/steamdeck.jpg"
  },
  {
    title: "Steam Gift Card",
    image: "images/giftcard.png"
  },
  {
    title: "Steam Controller",
    image: "images/controller.jpg"
  }
]
</script>

<template>
<section class="accessories" id="accessories">

    <h2>アクセサリー</h2>

    <div class="deck">
        <img src="/images/steamdeck.jpg" alt="Steam Deck">
    </div>

    <div class="accessory-grid">

        <div
            class="accessory-card"
            v-for="item in accessories.slice(1)"
            :key="item.title"
        >
            <img :src="item.image" :alt="item.title">

            <h3>{{ item.title }}</h3>

        </div>

    </div>

</section>
</template>

<style scoped>

</style>