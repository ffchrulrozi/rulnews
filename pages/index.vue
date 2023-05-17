<template>
  <div>
    <nav>
      <a href="#" class="">Home</a>
      <a href="#" class="">Trending</a>
      <a href="#" class="">Article</a>
    </nav>
    <section id="slider">
      <div class="slider-item"></div>
    </section>
    <section id="latest" class="grid grid-cols-6 gap-10">
      <div class="col-span-1 latest-category"></div>
      <div class="col-span-5">
        <div class="latest-item-header"></div>
        <div class="grid grid-cols-4 gap-5">
          <div
            class="latest-item"
            v-for="(latest, latestIndex) in latestExceptFirst"
            :key="latestIndex"
          ></div>
        </div>
      </div>
    </section>
    <section id="hot" class="grid grid-cols-5 gap-5">
      <div
        class="hot-item"
        v-for="(hot, hotIndex) in hots"
        :key="hotIndex"
      ></div>
    </section>
    <section id="promo">
      <div class="promo-area grid grid-cols-5 gap-5">
        <div
          class="promo-item"
          v-for="(promo, promoIndex) in promos"
          :key="promoIndex"
        ></div>
      </div>
    </section>
    <footer></footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      latests: [
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
        { title: '', desc: '', img: '' },
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
        { title: '', desc: '', img: '' },
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
  computed:{
    latestExceptFirst(){
      return this.latests.slice(1);
    }
  }
}
</script>

<style scoped>
</style>