<template>
  <div class="main">
    <PageHeader />
    <GirisYazisi />
    <DavetiyeLink />
    <YolTarifiHarita />
    <ConfettiExplosion />
  </div>
</template>

<script>
import VueConfetti from 'vue-confetti'
import Vue from 'vue'
Vue.use(VueConfetti)
export default {
  name: 'IndexPage',
  components: {
    PageHeader: () => import('@/components/PageHeader'),
    GirisYazisi: () => import('@/components/GirisYazisi'),
    DavetiyeLink: () => import('@/components/DavetiyeLink'),
    YolTarifiHarita: () => import('@/components/YolTarifiHarita'),
  },
  created() {
    this.$confetti.start({
      particles: [
        {
          type: 'heart',
        },
      ],
      defaultColors: ['red', 'pink', '#ba0000'],
    })
    setInterval(() => {
      this.$confetti.stop()
    }, 5000)
  },
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500&family=Roboto:wght@100;300&display=swap');
body {
  background-color: #fcf7ec;
}
.main {
  display: grid;
  justify-content: center;
  align-content: center;
  margin: auto;
  margin-top: 0px;
}
section {
  display: inline-block;
  padding: 0 10px 0px 10px;
  margin: 0px;
}
</style>
