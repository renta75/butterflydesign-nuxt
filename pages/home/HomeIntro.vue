<template>
  <div class="home">
    <div class="home__hero-section">
      <div class="home__hero-section-wrapper">
        <h1 class="home__hero-section-h1">Butterfly</h1>
        <h2 class="home__hero-section-h2 animate__animated animate__backInUp">
          Design
        </h2>
        <h3 class="home__hero-section-subheading">
          Product development studio
        </h3>
      </div>

      <div class="home__hero-section-butterfly">
        <img
          src="@/assets/Home-HeroButterfly.png"
          alt=""
          class="home__hero-section-butterfly-image"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeIntro",
  data() {
    return {
      anim: null,
    };
  },
  methods: {
    handleAnimation: function (anim) {
      this.anim = anim;
    },
  },
};

</script>

