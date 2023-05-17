<template>
  <div>
    <nav>
      <a href="#" class="">Home</a>
      <a href="#" class="">Trending</a>
      <a href="#" class="">Article</a>
    </nav>
    <section id="slider"></section>
    <section id="latest">
      <div class="latest-item" v-for="(latest, latestIndex) in latests" :key="latestIndex"></div>
    </section>
    <section id="hot" class="grid grid-cols-5 gap-5">
      <div class="hot-item" v-for="(hot, hotIndex) in hots" :key="hotIndex"></div>
    </section>
    <section id="promo">
      <div class="promo-area grid grid-cols-5 gap-5">
        <div
          class="promo-item"
          v-for="(promo, promoIndex) in promos"
          :key="promoIndex"
        >
        
        </div>
      </div>
    </section>
    <footer></footer>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      latests: [
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' }
      ],
      hots: [
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' }
      ],
      promos: [
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
      ],
    }
  },
}
</script>

<style scoped>
</style>