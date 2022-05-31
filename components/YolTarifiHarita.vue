<template>
  <div class="harita">
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d48770.394367780274!2d28.934500103513024!3d40.18348297443827!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x14ca16804f561671%3A0xbc912844accf9b9!2sAlt%C4%B1npark%20Tesisleri!5e0!3m2!1str!2str!4v1653989471380!5m2!1str!2str"
      width="390"
      height="450"
      style="border: 0"
      allowfullscreen=""
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"
    ></iframe>
    <br />
    <p class="tarif">Altınpark Tesisleri Orhaneli Yolu 6.KM Nilüfer/BURSA</p>
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
}
.tarif {
  text-align: center;
  font-size: 12pt;
  font-weight: bold;
}
</style>
