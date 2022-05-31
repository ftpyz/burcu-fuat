<template>
  <div class="harita">
    <p class="tarif">
      <span>Altınpark Tesisleri </span>
      <br />
      Orhaneli Yolu 6.KM Nilüfer/BURSA
      <br />
      <a
        target="_blank"
        href="https://maps.google.com/maps/dir//Alt%C4%B1npark+Tesisleri+G%C3%B6k%C3%A7e%C3%B6ren+Eski+Orhaneli+Yolu+6.+km+16110+Osmangazi%2FBursa/@40.1536991,28.9757911,12z/data=!4m5!4m4!1m0!1m2!1m1!1s0x14ca16804f561671:0xbc912844accf9b9"
        >Yol Tarifi Al</a
      >
    </p>

    <img src="~/static/harita.png" width="320" style="margin-left: 15%" />
  </div>
</template>
<script>
export default {
  name: 'YolTarifiHarita',
}
</script>
<style scoped>
p {
  font-family: 'Roboto', sans-serif;
  text-align: center;
  letter-spacing: 1px;
  word-spacing: 2px;
  margin: 10px 0px;
  padding: 10px 0px;
}
p span {
  font-size: 18pt;
  font-weight: bold;
}
p a {
  color: #000;
}
</style>
