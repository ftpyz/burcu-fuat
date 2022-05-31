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
          @click="degistir('kazdaglari')"
          src="~/static/mudanya.jpg"
        />

        <img
          :class="activeImg === 'kazdaglari' ? 'active' : ''"
          @click="degistir('kar')"
          src="~/static/kazdaglari.jpg"
        />
        <img
          :class="activeImg === 'kar' ? 'active' : ''"
          @click="degistir('sari')"
          src="~/static/kar.jpg"
        />
        <img
          :class="activeImg === 'sari' ? 'active' : ''"
          @click="degistir('kapadokya')"
          src="~/static/sari.jpg"
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
      interval: null,
      allImages: [
        'kapadokya',
        'bursa',
        'akyaka',
        'istanbul',
        'mudanya',
        'kazdaglari',
        'kar',
        'sari',
      ],
    }
  },
  created() {
    this.interval = setInterval(() => {
      const n = this.allImages[this.allImages.indexOf(this.activeImg) + 1]

      this.activeImg = n === undefined ? 'kapadokya' : n
    }, 3000)
  },
  methods: {
    degistir(id) {
      this.activeImg = id
      clearInterval(this.interval)
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
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.foto {
  margin-top: -20px;
  margin-left: -10px;
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
