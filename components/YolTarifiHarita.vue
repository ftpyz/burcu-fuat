<template>
  <div class="harita">
    <p class="tarif">
      <span>Altınpark Tesisleri </span>
      <br />
      Orhaneli Yolu 6.KM Nilüfer/BURSA
      <br />
      <a
        target="_blank"
        href="https://www.google.com/maps/dir/40.2194432,28.9865728/altınpark+tesisleri/@40.186611,28.9478482,13z/data=!3m1!4b1!4m9!4m8!1m1!4e1!1m5!1m1!1s0x14ca16804f561671:0xbc912844accf9b9!2m2!1d28.9757911!2d40.1536991"
        >Yol Tarifi Al</a
      >
    </p>
    <a
      href="https://www.google.com/maps/dir/40.2194432,28.9865728/altınpark+tesisleri/@40.186611,28.9478482,13z/data=!3m1!4b1!4m9!4m8!1m1!4e1!1m5!1m1!1s0x14ca16804f561671:0xbc912844accf9b9!2m2!1d28.9757911!2d40.1536991"
      target="_blank"
    >
      <img src="~/static/harita.png" width="390" />
    </a>
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
