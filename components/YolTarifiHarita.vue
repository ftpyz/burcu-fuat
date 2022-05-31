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
      href="https://www.google.com/maps/dir//alt%C4%B1npark+tesisleri/data=!4m6!4m5!1m1!4e2!1m2!1m1!1s0x14ca16804f561671:0xbc912844accf9b9?sa=X&ved=2ahUKEwjb38L1uYr4AhVXSPEDHY38CWoQ9Rd6BAhtEAU"
      target="_blank"
    >
      <div class="harita-resim">
        <a
          href="https://www.google.com/maps/dir//alt%C4%B1npark+tesisleri/data=!4m6!4m5!1m1!4e2!1m2!1m1!1s0x14ca16804f561671:0xbc912844accf9b9?sa=X&ved=2ahUKEwjb38L1uYr4AhVXSPEDHY38CWoQ9Rd6BAhtEAU"
          target="_blank"
          ><img src="~/static/harita.png" width="360" style="overflow: hidden"
        /></a>
      </div>
    </a>
  </div>
</template>
<script>
export default {
  name: 'YolTarifiHarita',
}
</script>
<style scoped>
.harita-resim {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
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
