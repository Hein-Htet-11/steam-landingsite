<script setup>
const communities = [
  {
    title: "Steam Reviews",
    text: "Read millions of reviews from players around the world.",
    stat: "30M+",
    label: "Reviews",
    link: "https://store.steampowered.com/reviews/"
  },
  {
    title: "Steam Community",
    text: "Join discussions, share screenshots and connect with players.",
    stat: "100M+",
    label: "Members",
    link: "https://steamcommunity.com/"
  }
]
</script>

<template>

<section class="community" id="community">

    <div class="community-info">

        <h2>コミュニティ</h2>

        <h1>
            世界中のプレイヤーと<br>
            交流しよう
        </h1>

        <p>
            Join millions of Steam users, write reviews,
            share screenshots and enjoy games together.
        </p>

    </div>

    <div class="community-cards">

        <a
            class="community-card"
            v-for="item in communities"
            :key="item.title"
            :href="item.link"
            target="_blank"
        >

            <h3>{{ item.title }}</h3>

            <p>{{ item.text }}</p>

            <span class="community-number">
                {{ item.stat }}
            </span>

            <small>{{ item.label }}</small>

            <div class="community-link">
                Visit →
            </div>

        </a>

    </div>

</section>

</template>

<style scoped>

</style>