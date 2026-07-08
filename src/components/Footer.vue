<template>
<footer class="footer">

    <div class="footer-logo">

        <img src="/images/steam-logo.png" alt="Steam Logo">

        <h2>STEAM</h2>

    </div>

    <div class="footer-links">

        <a href="#about">Steamについて</a>
        <a href="#games">ゲーム一覧</a>
        <a href="#accessories">アクセサリー</a>
        <a href="#community">コミュニティ</a>
        <a href="#support">サポート</a>

    </div>

    <div class="copyright">
        © 2026 HEIN HTET ZIN
    </div>

</footer>
</template>

<style scoped>

.footer{
    background:#101010;
    text-align:center;
    padding:50px 20px;
}

.footer-logo img{
    width:70px;
    margin:auto;
}

.footer-logo h2{
    margin:15px 0 30px;
}

.footer-links{
    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;
    margin-bottom:30px;
}

.footer-links a{
    color:#bbb;
    transition:.3s;
}

.footer-links a:hover{
    color:#66c0f4;
}

.copyright{
    color:#777;
    font-size:14px;
}

</style>