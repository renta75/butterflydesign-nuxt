<template>
    <div class="section4">
        <div class="container section4__section4-wrapper">
            <div class="section4__title-wrapper">
                <h1 class="section4__section4-h1">SMART SOLUTIONS ABOVE </h1>
                <h2 class="section4__section4-h2">ALL EXPECTATIONS</h2>
            </div>

            <div class="section4__section4-content-wrapper">
                <p class="section4__text">
                    We look at every product as our<span style="color: #ff18f7">biggest accomplishment.</span>
                </p>
                <p class="section4__text">
                    Our goal is to make even the craziest of <span style="color: #ff18f7">our client's </span> ideas come to life.
                </p>
                <p class="section4__text">
                    Are you ready to meet the technology-loving, innovation driven team behind <span style="color: #ff18f7">Butterfly Design?</span>
                </p>

                <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="section4__button"><span>CONTACT US</span></NuxtLink>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HomeSectionFour'
}
</script>