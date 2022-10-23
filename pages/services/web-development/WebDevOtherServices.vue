<template>
    <div class="web-development__main-section__other-services">
        <h2 class="web-development__main-section__other-services-h2"> Our other services </h2>

        <div class="web-development__main-section__other-services-wrapper">
            <NuxtLink to="/services/maintenance" class="web-development__main-section__other-service">
                <img src="@/assets/services/Services-E-commerce-Icon.png" alt="">
                <h4 class="web-development__main-section__other-service-heading"><span>E-COMMERCE</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/maintenance" class="web-development__main-section__other-service">
                <img src="@/assets/services/Services-Maintenance-Icon.png" alt="">
                <h4 class="web-development__main-section__other-service-heading"><span>MAINTENANCE</span></h4>
            </NuxtLink>

            <NuxtLink to="/services/graphic-design" class="web-development__main-section__other-service">
                <img src="@/assets/services/Services-GraphicDesign-Icon.png" alt="">
                <h4 class="web-development__main-section__other-service-heading"><span>GRAPHIC DESIGN</span></h4>
            </NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    name: 'WebDevOtherServices'
}
</script>