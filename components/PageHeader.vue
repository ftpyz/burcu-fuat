<template>
  <section>
    <div class="cicek">
      <div class="foto">
        <img class="active" src="~/static/kapadokya-1.jpg" />
        <img class="" src="~/static/bursa-1.jpg" />
        <img class="" src="~/static/akyaka.jpg" />
        <img class="" src="~/static/istanbul.jpg" />
      </div>
    </div>
  </section>
</template>
<script>
// Import Swiper styles
export default {
  name: 'PageHeader',
}
</script>
<style scoped>
.cicek {
  background-image: url('static/cicekler.png');
  width: 320px;
  height: 320px;
  margin: auto;
}
.foto {
  z-index: 10;
  position: relative;
  left: 28%;
  top: 27%;
}
.foto img {
  opacity: 0.8;
  border-radius: 140px;
  width: 130px;
  height: 130px;
  display: none;
}
.foto img.active {
  display: block;
}
</style>
