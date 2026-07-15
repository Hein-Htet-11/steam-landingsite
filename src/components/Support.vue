<script setup>
const supports = [
  {
    icon: "FAQ",
    title: "FAQ",
    text: "Find answers to common questions.",
    url: "https://help.steampowered.com/"
  },
  {
    icon: "CONTACT",
    title: "Contact Us",
    text: "Send us your questions or feedback.",
    url: "#contact"
},
  {
    icon: "FORUM",
    title: "Community Help",
    text: "Ask other Steam players for help.",
    url: "https://steamcommunity.com/discussions/"
  }
]
</script>

<template>
<section class="support" id="support">

    <h2>サポート</h2>

    <p class="support-text">
        Need help? Our support team is here to assist you.
    </p>

    <div class="support-grid">

    <a
    v-for="item in supports"
    :key="item.title"
    :href="item.url"
    :target="item.url.startsWith('http') ? '_blank' : null"
    class="support-card"
>

    <div class="icon">
        {{ item.icon }}
    </div>

    <h3>{{ item.title }}</h3>

    <p>{{ item.text }}</p>

    <span class="learn-more">
        Learn More →
    </span>

</a>

    </div>

</section>
</template>

<style scoped>

</style>