<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value
}

const closeMenu = () => {
  menuOpen.value = false
}
</script>

<template>

<header class="header">

    <div class="logo">
        <img src="/images/steam-logo.png" alt="Steam Logo">
    </div>

    <button
        class="menu-btn"
        @click="toggleMenu"
    >
        {{ menuOpen ? "✕" : "☰" }}
    </button>

    <nav :class="{ active: menuOpen }">

        <ul>

            <li>
                <a href="#about" @click="closeMenu">Steamについて</a>
            </li>

            <li>
                <a href="#games" @click="closeMenu">ゲーム一覧</a>
            </li>

            <li>
                <a href="#accessories" @click="closeMenu">アクセサリー</a>
            </li>

            <li>
                <a href="#community" @click="closeMenu">コミュニティ</a>
            </li>

            <li>
                <a href="#support" @click="closeMenu">サポート</a>
            </li>

            <li>
                <a href="#contact" @click="closeMenu">連絡</a>
            </li>

        </ul>

    </nav>

</header>

</template>

<style scoped>

.header{

    background:#000;

    display:flex;

    justify-content:space-between;

    align-items:center;

    padding:20px 50px;

    position:sticky;

    top:0;

    z-index:1000;
}

.logo img{

    width:90px;
}

ul{

    display:flex;

    gap:40px;

    list-style:none;
}

a{

    color:white;

    text-decoration:none;

    font-weight:bold;

    transition:.3s;
}

a:hover{

    color:#66c0f4;
}

.menu-btn{

    display:none;

    background:none;

    border:none;

    color:white;

    font-size:32px;

    cursor:pointer;
}

/* ---------- Mobile ---------- */

@media (max-width:768px){

    .header{

        padding:18px 25px;
    }

    .menu-btn{

        display:block;
    }

    nav{

        position:absolute;

        top:100%;

        left:0;

        width:100%;

        background:#000;

        max-height:0;

        overflow:hidden;

        transition:max-height .35s ease;
    }

    nav.active{

        max-height:500px;
    }

    ul{

        flex-direction:column;

        align-items:center;

        gap:25px;

        padding:30px 0;
    }

}

</style>