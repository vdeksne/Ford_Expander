<template>
  <section class="section-video">
    <ExpanderVideo
      filename="1080.mp4"
      :autoplay="true"
      url="https://secure.adnxs.com/clktrb?id=806640&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.396947846;dc_trk_aid=588724183;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
    />
  </section>

  <div class="blue-line"></div>

  <section class="section-main">
    <div class="text">
      <h1 class="heading">
        <strong>F-150</strong>
        LIGHTNING
      </h1>
      <p class="lead">VÅR IMPONERENDE HELELEKTRISKE PICKUP</p>
      <p>
        F-150 Lightning er vår første helelektriske pickup – med 5 seter, god
        rekkevidde, 3,5 tonn tilhengervekt og enorm plass. Norsk presse har latt
        seg begeistre og skriver blant annet "Rett og slett en imponerende bil"
        (TV 2 Broom) og "If bigger is better, this is perfect" (Finansavisen).
        Prøv den du også – og finn ut om du er enig.
      </p>
      <div class="actions">
        <a
          href="https://secure.adnxs.com/clktrb?id=806641&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.396949625;dc_trk_aid=588734352;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
          target="_blank"
          class="cta"
        >
          Be om prøvekjøring
        </a>
        <a
          href="https://secure.adnxs.com/clktrb?id=806642&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.397231263;dc_trk_aid=588734355;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
          target="_blank"
          class="cta"
        >
          Finn din forhandler
        </a>
      </div>
    </div>
    <a
      href="https://secure.adnxs.com/clktrb?id=802715&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B31787091.391082153;dc_trk_aid=582555944;dc_trk_cid=212504900;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
      target="_blank"
      class="image"
    >
      <img src="@/assets/image-1.jpg" />
    </a>
  </section>

  <section class="section-details">
    <div class="items">
      <div class="item">
        <div class="label">ELEKTRISK REKKEVIDDE (WLTP)</div>
        <div class="value">429 KM</div>
      </div>
      <div class="item">
        <div class="label">0-100 KM/T</div>
        <div class="value">>5 SEK</div>
      </div>
      <div class="item">
        <div class="label">15-80% HURTIGLADING</div>
        <div class="value">39 MIN</div>
      </div>
    </div>
    <a
      href="https://secure.adnxs.com/clktrb?id=802715&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B31787091.391082153;dc_trk_aid=582555944;dc_trk_cid=212504900;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
      target="_blank"
      class="price"
    >
      <div class="label">Veil.pris fra</div>
      <div class="value">1 072 500 NOK</div>
    </a>
  </section>

  <section class="section-slider">
    <ExpanderSlider @track="track" />
    <div class="logo">
      <img src="@/assets/f150.png" />
      <p class="phrase">So Much Power, So Many Possibilities.</p>
    </div>
  </section>

  <section class="section-scroller">
    <ExpanderSliderAlt />
  </section>

  <footer class="section-footer">
    <a
      href="https://secure.adnxs.com/clktrb?id=806647&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.396947846;dc_trk_aid=588724183;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
      target="_blank"
      class="logo"
    >
      <img src="@/assets/ford.svg" />
    </a>
  </footer>

  <footer class="footer">
    <div class="actions">
      <a
        href="https://secure.adnxs.com/clktrb?id=806643&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.396949625;dc_trk_aid=588734352;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
        target="_blank"
        class="cta-2"
        >Be om prøvekjøring</a
      >
      <a
        href="https://secure.adnxs.com/clktrb?id=806644&redir=https://ad.doubleclick.net/ddm/trackclk/N9166.4661577SHOWHEROESNO/B32127914.397231263;dc_trk_aid=588734355;dc_trk_cid=216809167;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1"
        target="_blank"
        class="cta-2"
      >
        Finn din forhandler
      </a>
    </div>
  </footer>
</template>

<script>
import ExpanderVideo from "./components/ExpanderVideo.vue";
import ExpanderSlider from "./components/ExpanderSlider.vue";
import ExpanderSliderAlt from "./components/ExpanderSliderAlt.vue";

export default {
  name: "App",
  components: {
    ExpanderVideo,
    ExpanderSlider,
    ExpanderSliderAlt,
  },
  data() {
    return {
      mobile: false,
    };
  },
  created() {
    if (window.innerWidth < 480) {
      this.mobile = true;
    }
  },
  methods: {
    track(label) {
      return label;
    },
  },
};
</script>

<style lang="scss">
@import "node_modules/minireset.css/minireset";
@import "@/scss/fonts.scss";
@import "@/scss/variables.scss";
@import "@/scss/mixins.scss";

html {
  font-family: $font, sans-serif;
  font-size: 16px;
  font-weight: $weight;
  color: $color-text;
  text-align: left;
  line-height: 1.3;
  @include desktop {
    font-size: 1.48vw;
  }
  @media (min-width: $width) {
    font-size: 16px;
  }
}
#app {
  position: relative;
  width: $width;
  max-width: 100%;
  margin: 0 auto;
  background: $color-bg;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

img {
  display: block;
}
a {
  color: inherit;
  text-decoration: none;
}
p {
  font-size: 1rem;
}
button {
  font-family: $font;
  font-size: 1rem;
  padding: 0;
  border: 0;
  background: none;
  outline: 0 none;
  cursor: pointer;
}

.cta {
  display: inline-block;
  padding: 0.8125rem 1.625rem;
  font-size: 1rem;
  color: #fff;
  background: $color-1;
  border-radius: 3.25rem;
  transition: 0.15s;
  &:hover {
    background: $color-2;
  }
}
.cta-2 {
  display: inline-block;
  padding: 0.8125rem 1.625rem;
  font-size: 1rem;
  color: $color-1;
  background: #fff;
  border-radius: 3.25rem;
  transition: 0.15s;
  &:hover {
    scale: 1.1;
  }
  margin: 3rem;
  transition: all 0.3s ease-in-out;
}

.blue-line {
  height: 1.3125rem;
  width: 100%;
  background: $color-1;
}

.footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  text-align: center;
  z-index: 1000;
  height: 7.1875rem;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #102b4e;
  @include m {
    height: 4rem;
  }
  .actions {
    @include m {
      display: flex;
      padding: 0 1rem;
      a {
        margin: 0 .5rem;
        padding: 0.5rem .625rem;
        font-size: .875rem;
      }
    }
  }
}
</style>

<style scoped lang="scss">
@import "@/scss/variables.scss";
@import "@/scss/mixins.scss";

.section-main {
  @include d {
    display: flex;
    justify-content: space-between;
    .text {
      width: 31.125rem;
    }
    .image {
      width: 36.375rem;
    }
  }
  .text {
    padding: 2rem 2rem;
    @include d {
      padding: 2rem 2rem 2rem 4.125rem;
    }
    .heading {
      margin-bottom: 1rem;
      font-size: 2.25rem;
      color: $color-1;
      line-height: 1;
      @include d {
        margin-bottom: 1.5rem;
        font-size: 3.25rem;
      }
      strong {
        display: block;
        font-weight: bold;
      }
    }
    p {
      font-size: 1rem;
      font-weight: 300;
    }
    p + p {
      margin-top: 1.25rem;
    }
    .lead {
      font-weight: bold;
      font-size: 1.5rem;
    }
    .actions {
      margin-top: 1.625rem;
      display: flex;
      .cta {
        padding: 0.8125rem 1.625rem;
        font-size: 0.875rem;
        @include m {
          padding: 0.8125rem 1.25rem;
          font-size: 0.75rem;
        }
      }
      .cta + .cta {
        margin-left: 0.625rem;
      }
    }
  }
}

.section-details {
  position: relative;
  z-index: 2;
  padding: 14rem 2.5rem 14.5rem;
  margin: -15rem 0 -15.5rem;
  color: #fff;
  background: url("@/assets/bg.svg") no-repeat center top / cover;
  @include d {
    padding: 13rem 12.75rem 14.5rem;
  }
  .items {
    @include d {
      display: flex;
      justify-content: space-between;
      align-items: end;
    }
    .item {
      max-width: 11.25rem;
      margin: 0 auto 2rem;
      text-align: center;
      @include d {
        margin: 0;
        text-align: left;
      }
      .label {
        margin-bottom: 0.375rem;
        font-weight: 300;
      }
      .value {
        font-family: "Ford Antenna Cond";
        font-size: 1.5rem;
        font-weight: bold;
      }
    }
  }
  .price {
    display: block;
    width: 16.875rem;
    padding: 0.875rem;
    margin: 1.375rem auto 0;
    text-align: center;
    border-radius: 0.33781rem;
    border: 0.386px solid rgba(255, 255, 255, 0.54);
    background: rgba(255, 255, 255, 0.02);
    backdrop-filter: blur(10.731908798217773px);
    transition: 0.15s;
    &:hover {
      background: #fff;
      color: $color-1;
    }
    .label {
      font-size: 0.75rem;
    }
    .value {
      font-size: 1.75rem;
      font-weight: bold;
    }
  }
}

.section-slider {
  position: relative;
  z-index: 3;
  @include m {
    padding-bottom: 10rem;
  }
  .logo {
    position: absolute;
    z-index: 10;
    right: 3rem;
    bottom: 1rem;
    width: 28.375rem;
    @include m {
      width: 18rem;
      right: 1rem;
      bottom: 2.5625rem;
    }
    .phrase {
      margin-top: 1rem;
      margin-right: 1.5rem;
      font-size: 2rem;
      font-weight: bold;
      color: $color-1;
      text-align: right;
      @include m {
        margin-right: 0.5rem;
        font-size: 1.5rem;
      }
    }
  }
}

.section-footer {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 5rem 2rem;
  background: $color-1;
  @include d {
    padding: 13.125rem 2rem;
  }
  .logo {
    width: 15rem;
    @include d {
      width: 25.25rem;
    }
  }
}
</style>
