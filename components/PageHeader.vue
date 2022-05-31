<template>
  <section>
    <div class="cicek">
      <div class="foto" ref="sliders">
        <img
          :class="activeImg === 'kapadokya' ? 'active' : ''"
          @click="degistir('bursa')"
          src="~/static/kapadokya-1.jpg"
        />
        <img
          :class="activeImg === 'bursa' ? 'active' : ''"
          @click="degistir('akyaka')"
          src="~/static/bursa-1.jpg"
        />
        <img
          :class="activeImg === 'akyaka' ? 'active' : ''"
          @click="degistir('istanbul')"
          src="~/static/akyaka.jpg"
        />
        <img
          :class="activeImg === 'istanbul' ? 'active' : ''"
          @click="degistir('mudanya')"
          src="~/static/istanbul.jpg"
        />
        <img
          :class="activeImg === 'mudanya' ? 'active' : ''"
          @click="degistir('kapadokya')"
          src="~/static/mudanya.jpg"
        />
      </div>
    </div>
  </section>
</template>
<script>
// Import Swiper styles
export default {
  name: 'PageHeader',

  data() {
    return {
      activeImg: 'kapadokya',
      allImages: ['kapadokya', 'bursa', 'akyaka', 'istanbul', 'mudanya'],
    }
  },
  created() {
    setInterval(() => {
      const n = this.allImages[this.allImages.indexOf(this.activeImg) + 1]
      this.activeImg = n
    }, 3000)
  },
  methods: {
    degistir(id) {
      this.activeImg = id
    },
  },
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
