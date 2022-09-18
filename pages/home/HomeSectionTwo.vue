<template>
  <div class="container section2">
    <div class="laptop">
      <img
        src="@/assets/Laptop-Webdevelopment.png"
        alt=""
        class="laptop__image"
      />
      <div class="laptop__content">
        <h3 class="laptop__heading">App Development <span class="makni">GGGGG</span></h3>
        <p class="laptop__text">
          We create websites from concept to implementation. We are actively
          involved in all the steps required to create your project.
        </p>
        <NuxtLink to="/services/web-development" class="laptop__link"
          >Read More...</NuxtLink
        >
      </div>
    </div>
    <div class="laptop">
      <img src="@/assets/Laptop-eCommerce.png" alt="" class="laptop__image" />
      <div class="laptop__content">
        <h3 class="laptop__heading">ECommerce Sites & Apps</h3>
        <p class="laptop__text">
          End to end e-commerce solutions to start, grow and expand your online
          business.
        </p>
        <NuxtLink to="/services/e-commerce" class="laptop__link"
          >Read More...</NuxtLink
        >
      </div>
    </div>
    <div class="laptop">
      <img src="@/assets/Laptop-Maintenance.png" alt="" class="laptop__image" />
      <div class="laptop__content">
        <h3 class="laptop__heading">Maintaining Sites & Apps</h3>
        <p class="laptop__text">
          WordPress website maintenance, optimization, recovery, fixes and
          support.
        </p>
        <NuxtLink to="/services/maintenance" class="laptop__link"
          >Read More...</NuxtLink
        >
      </div>
    </div>
    <div class="laptop">
      <img
        src="@/assets/Laptop-GraphicDesign.png"
        alt=""
        class="laptop__image"
      />
      <div class="laptop__content">
        <h3 class="laptop__heading">UI/UX Design Apps & Sites</h3>
        <p class="laptop__text">
          Logo Design and marketing materials printed and delivered to your
          door.
        </p>
        <NuxtLink to="/services/graphic-design" class="laptop__link"
          >Read More...</NuxtLink
        >
      </div>
    </div>
  </div>
</template>

