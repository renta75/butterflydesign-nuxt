<template>
    <div class="graphic-design__main-section__other-services">
        <h2 class="graphic-design__main-section__other-services-h2">Check other services</h2>

        <div class="graphic-design__main-section__other-services-wrapper">
            <NuxtLink to="/services/web-development" class="graphic-design__main-section__other-service">
                <img src="@/assets/services/Services-Development-Icon.png" alt="">
                <h4 class="graphic-design__main-section__other-service-heading"><span>DEVELOPMENT</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/e-commerce" class="graphic-design__main-section__other-service">
                <img src="@/assets/services/Services-E-commerce-Icon.png" alt="">
                <h4 class="graphic-design__main-section__other-service-heading"><span>E-COMMERCE</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/maintenance" class="graphic-design__main-section__other-service">
                <img src="@/assets/services/Services-Maintenance-Icon.png" alt="">
                <h4 class="graphic-design__main-section__other-service-heading"><span>MAINTENANCE</span></h4>
            </NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    name: 'GraphicDesignOtherServices'
}
</script>