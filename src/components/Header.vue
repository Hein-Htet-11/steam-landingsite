<template>
  <header class="header">
    <div class="logo">
      <img src="/images/steam-logo.png" alt="Steam Logo">
    </div>

    <nav>
      <ul>
        <li><a href="#about">Steamについて</a></li>
        <li><a href="#games">ゲーム一覧</a></li>
        <li><a href="#accessories">アクセサリー</a></li>
        <li><a href="#community">コミュニティ</a></li>
        <li><a href="#support">サポート</a></li>
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
}

.logo img{
    width:90px;
}

ul{
    display:flex;
    list-style:none;
    gap:40px;
}

a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

a:hover{
    color:#66c0f4;
}
</style>