<template>
  <div class="website-wrapper">
    <header-global class="header"/>
    <transition name="fade" mode="out-in" >
      <Nuxt @hook:mounted="makeSomeStuff" />
    </transition>
    <footer-global v-if="mounted" class="footer"  />
  </div>
</template>

<script>
import HeaderGlobal from "../components/Header.vue";
import FooterGlobal from "../components/Footer.vue";

export default {
  components: {
    HeaderGlobal,
    FooterGlobal
  },
  data: () => ({
    mounted: false
  }),
  methods: {
    makeSomeStuff() {
      this.mounted = true;
    }
  }, 
  metaInfo: {
    title: "Butterfly Design",
    meta: [
      { charset: "utf-8" },
      {
        name: "viewport",
        content: "width=device-width, initial-scale=1, user-scalable=no",
      },
    ],
    htmlAttrs: {
      lang: "en",
      amp: true,
    },
  },
};

</script>

<style lang="scss">
@import "@/assets/scss/_main.scss";
.fade-enter-active,
.fade-leave-active {
  transition-property: opacity;
  transition-duration: 0.3s;
}

.fade-enter-active {
  transition-delay: 0.3s;
}

.fade-enter,
.fade-leave-active {
  opacity: 0;
}

body::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.6);
  background-color: #4700cc;
}

body::-webkit-scrollbar {
  width: 10px;
  background-color: #f5f5f5;
}

body::-webkit-scrollbar-thumb {
  background-color: #fff;
  background-image: linear-gradient(
    45deg,
    rgb(22, 255, 255) 0%,
    rgb(255, 24, 247) 100%
  );
}
</style>
