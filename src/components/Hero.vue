<template>
  <section class="hero">
    <img
      src="/images/autumn-sale.jpg"
      alt="Autumn Sale"
      class="hero-image"
    >

    <div class="hero-text">
      <h1>Autumn Sale</h1>
      <p>Explore thousands of games on Steam.</p>
      <button>Browse Games</button>
    </div>
  </section>
</template>

<style scoped>
.hero{
    position:relative;
    width:100%;
}

.hero-image{
    width:100%;
    display:block;
}

.hero-text{
    position:absolute;
    top:50%;
    left:8%;
    transform:translateY(-50%);
    color:white;
}

.hero-text h1{
    font-size:64px;
    margin-bottom:10px;
}

.hero-text p{
    font-size:22px;
    margin-bottom:20px;
}

button{
    background:#66c0f4;
    color:white;
    border:none;
    padding:12px 24px;
    border-radius:8px;
    cursor:pointer;
    font-size:18px;
    transition:.3s;
}

button:hover{
    background:#4aa8dd;
}
</style>