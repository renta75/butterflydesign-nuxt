<template>
    <div class="container services-wrapper">
        <div class="services-wrapper__box">
            <img class="services-wrapper__top-img" src="@/assets/services/Services-Development-Icon.png" alt="">
            <h3 class="services-wrapper__heading">Development</h3>
            <p class="services-wrapper__text">We take advantage of top-notch technology and implement that professional knowledge in every product we create. With clean code, we can create fully responsive websites that users love on every type of chosen device. Every step of the development process is fully customizable to our client's wishes and needs.
            </p>
            <NuxtLink to="/services/web-development" class="services-wrapper__link"><span>Read More</span></NuxtLink>
        </div>
        <div class="services-wrapper__box">
            <img class="services-wrapper__top-img" src="@/assets/services/Services-E-commerce-Icon.png" alt="">
            <h3 class="services-wrapper__heading">E-commerce</h3>
            <p class="services-wrapper__text">Online shopping has never been more popular. Studies have shown that more people today are willing to shop online than physically go to a store. That is why we discover, analyse, compile, and, at the end, create amazing websites that both our clients and their users completely fall in love with.
            </p>
            <NuxtLink to="/services/e-commerce" class="services-wrapper__link"><span>Read More</span></NuxtLink>
        </div>
        <div class="services-wrapper__box">
            <img class="services-wrapper__top-img" src="@/assets/services/Services-Maintenance-Icon.png" alt="">
            <h3 class="services-wrapper__heading">Maintenance</h3>
            <p class="services-wrapper__text">Protection and security are our priorities. We make sure you never lose any information crucial to your business which will help you put your efforts into the growth of your business, and thus prevent any unnecessary worry over technicalities. Consistent data protection, organization, and storage are a must for every 
            </p>
            <NuxtLink to="/services/maintenance" class="services-wrapper__link"><span>Read More</span></NuxtLink>
        </div>
        <div class="services-wrapper__box">
            <img class="services-wrapper__top-img" src="@/assets/services/Services-GraphicDesign-Icon.png" alt="">
            <h3 class="services-wrapper__heading">UI/UX DESIGN</h3>
            <p class="services-wrapper__text">Design is not just about putting together beautiful colors and shapes, it is also about digging deep and understanding current trends, analysing your business goals, and working with your user's psychological understanding to provide the best possible user experience. With our knowledge, we build designs that users love to come back to.
            </p>
            <NuxtLink to="/services/graphic-design" class="services-wrapper__link"><span>Read More</span></NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ServicesBoxes'
}
</script>