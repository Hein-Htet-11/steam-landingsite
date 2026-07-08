<template>
  <section class="hero">

    <img
      src="/images/autumn-sale.jpg"
      alt="Autumn Sale"
      class="hero-image"
    >

    <div class="hero-overlay"></div>

    <div class="hero-text">

      <span class="hero-badge">
        LIMITED TIME EVENT
      </span>

      <h1>AUTUMN SALE</h1>

      <p>
        Discover thousands of games,
        exclusive discounts and the world's
        largest PC gaming community.
      </p>

      <div class="hero-buttons">

        <a href="#games" class="primary-btn">
          Browse Games
        </a>

        <a
          href="https://store.steampowered.com/"
          target="_blank"
          class="secondary-btn"
        >
          Visit Steam
        </a>

      </div>

      <div class="hero-stats">

        <div>
          <strong>130K+</strong>
          <span>Games</span>
        </div>

        <div>
          <strong>40M+</strong>
          <span>Players</span>
        </div>

        <div>
          <strong>★★★★★</strong>
          <span>Top Platform</span>
        </div>

      </div>

    </div>

  </section>
</template>
<style scoped>

.hero{
    position:relative;
    overflow:hidden;
}

.hero-image{
    width:100%;
    height:700px;
    object-fit:cover;
    display:block;
}

.hero-overlay{
    position:absolute;
    inset:0;
    background:rgba(0,0,0,.45);
}

.hero-text{
    position:absolute;
    top:50%;
    left:8%;
    transform:translateY(-50%);
    max-width:620px;
    z-index:2;
}

.hero-badge{
    display:inline-block;
    padding:8px 18px;
    border:1px solid #66c0f4;
    color:#66c0f4;
    border-radius:999px;
    font-size:13px;
    font-weight:700;
    letter-spacing:1.5px;
    text-transform:uppercase;
    margin-bottom:20px;
}

.hero-text h1{
    font-size:72px;
    line-height:1;
    margin-bottom:25px;
}

.hero-text p{
    font-size:22px;
    color:#ddd;
    margin-bottom:35px;
}

.hero-buttons{
    display:flex;
    gap:18px;
    margin-bottom:45px;
}

.primary-btn,
.secondary-btn{

    padding:14px 28px;
    border-radius:10px;
    transition:.3s;
    font-weight:bold;
}

.primary-btn{
    background:#66c0f4;
}

.primary-btn:hover{
    background:#4bace8;
}

.secondary-btn{

    border:2px solid white;
}

.secondary-btn:hover{

    background:white;
    color:#171a21;
}

.hero-stats{

    display:flex;
    gap:45px;
}

.hero-stats div{

    display:flex;
    flex-direction:column;
}

.hero-stats strong{

    font-size:24px;
}

.hero-stats span{

    color:#b8b8b8;
    font-size:14px;
}

</style>