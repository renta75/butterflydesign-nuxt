<template>
    <div class="ecommerce__bottom-section__other-services">
        <h2 class="ecommerce__bottom-section__other-services-h2">Our other services</h2>

        <div class="ecommerce__bottom-section__other-services-wrapper">
            <NuxtLink to="/services/web-development" class="ecommerce__bottom-section__other-service">
                <img src="@/assets/services/Services-Development-Icon.png" alt="">
                <h4 class="ecommerce__bottom-section__other-service-heading"><span>DEVELOPMENT</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/maintenance" class="ecommerce__bottom-section__other-service">
                <img src="@/assets/services/Services-Maintenance-Icon.png" alt="">
                <h4 class="ecommerce__bottom-section__other-service-heading"><span>MAINTENANCE</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/graphic-design" class="ecommerce__bottom-section__other-service">
                <img src="@/assets/services/Services-GraphicDesign-Icon.png" alt="">
                <h4 class="ecommerce__bottom-section__other-service-heading"><span>GRAPHIC DESIGN</span></h4>
            </NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ECommerceOtherServices'
}
</script>