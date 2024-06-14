<template>
  <div class="wrapper">
    <div class="slider" ref="slider">
      <article class="item" v-for="item in items" :key="item">
        <img :src="getImage(item)" />
      </article>
    </div>

    <div class="overlay">
      <h1 class="heading">F-150</h1>
      <h2 class="subheading">LIGHTNING</h2>
    </div>

  </div>
</template>

<script>
import { tns } from "tiny-slider";

export default {
  name: "ExpanderSliderAlt",
  emits: ["track"],
  data() {
    return {
      items: [
        'image-1.jpg',
        'image-2.jpg',
      ]
    };
  },
  mounted() {
    tns({
      container: this.$refs.slider,
      items: 1,
      gutter: 0,
      mode: 'gallery',
      controls: false,
      nav: false,
      autoplay: true,
      autoplayTimeout: 3000,
      autoplayButtonOutput: false,
      speed: 500,
      loop: true
    });
  },
  methods: {
    getImage(image) {
      return require(`@/assets/bottom/${image}`);
    },
  },
};
</script>

<style lang="scss">
@import "node_modules/tiny-slider/src/tiny-slider";
</style>

<style scoped lang="scss">
@import "@/scss/variables.scss";
@import "@/scss/mixins.scss";

.wrapper {
  position: relative;
  background: #000;

  .overlay {
    position: absolute;
    left: 0;
    top: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100%;
    width: 22rem;
    padding-left: 2.5rem;
    color: #fff;
    background: linear-gradient(to left, rgba(0, 0, 0, 0.00) 0%, #080912 100%);
    @include m {
      width: 50%;
      padding-left: 1.5rem;
    }
    .heading {
      font-size: 3.25rem;
      font-weight: bold;
      @include m {
        font-size: 1.5rem;
      }
    }
    .subheading {
      margin-top: -.5rem;
      font-size: 3.25rem;
      font-weight: normal;
      @include m {
        font-size: 1.5rem;
      }
    }
  }

}
</style>
