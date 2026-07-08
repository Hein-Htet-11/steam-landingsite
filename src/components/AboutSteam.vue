<template>
  <section class="about" id="about">
    <div class="logo">
      <img src="/images/steam-white.png" alt="Steam Logo">
    </div>

    <div class="content">
      <h2>STEAM</h2>

      <p>
        Steamは世界中で利用されているPCゲーム配信サービスです。
      </p>

      <p>
        多くのゲームを購入・ダウンロードでき、
        レビューやコミュニティ機能も利用できます。
      </p>
    </div>
  </section>
</template>

<style scoped>

.about{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:50px;

    background:#1d1d1d;
    color:white;

    padding:70px 100px;
}

.logo img{
    width:220px;
}

.content{
    max-width:700px;
}

.content h2{
    font-size:48px;
    margin-bottom:20px;
}

.content p{
    font-size:22px;
    line-height:1.8;
}

</style>