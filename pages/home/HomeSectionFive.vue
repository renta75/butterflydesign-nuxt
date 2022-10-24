<template>
    <div class="section5">
        <div class="container">
            <div class="elevated-boxes">
                <div class="elevated-boxes__wrapper">
                    <div>
                        <img
                            class="elevated-boxes__top-img first-img"
                            src="@/assets/Home-Leptir.png"
                            alt=""
                        />
                        <h3>Why butterfly design?</h3>
                        <p>
                            Butterflies go through complete metamorphosis. This means that there are five parts in a butterfly's life just as we believe there are five main points in a majorly successful design: research, ideation, realization, implementation, and testing.
                        </p>
                    </div>
                    <div class="elevated-boxes__elevated-box">
                        <img
                            class="elevated-boxes__top-img"
                            src="@/assets/Home-Target.png"
                            alt=""
                        />
                        <h3>MISSION AND VISION</h3>
                        <p>
                            Studies have shown that design has a major impact on business success. That is why our mission is to help set businesses up for victory. No matter the age, tech intellect, or other specifics of your users, we create products that accommodate every person.
                        </p>
                    </div>
                    <div>
                        <img
                            class="elevated-boxes__top-img"
                            src="@/assets/Home-Puzzle.png"
                            alt=""
                        />
                        <h3>ABOUT US</h3>
                        <p>
                            We love to help small and medium-sized businesses receive awesome products and realize they can have a major impact by implementing banging visual identities online. Overdelivering is our standard because we don’t just work for our clients, we truly care for their success.

                        </p>
                    </div>
                </div>
            </div>

            <div class="section5__contact">
                <NuxtLink to="/about" class="section5__button"><span>GET TO KNOW US</span></NuxtLink>

                <h3 class="section5__contact__heading">Let’s build outstanding products together</h3>

                <div class="section5__contact__text">
                    <span>Project consulting</span>
                    <span class="section5__contact__slash"></span>
                    <span>Product reviving</span>
                    <span class="section5__contact__slash"></span>
                    <span>Long term support</span>
                </div>

                <div class="section5__contact__buttons">
                    <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="section5__button-email"><img src="@/assets/Button-Email.svg" alt="" class="section5__contact__icon"><span>info@butterflydesign.hr</span></NuxtLink>
                    <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="section5__button-phone"><img src="@/assets/Button-Phone.svg" alt="" class="section5__contact__icon phone-icon"><span>+385914777020</span></NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HomeSectionFive'
}
</script>