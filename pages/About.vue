<template>
    <div class="about">
        <about-intro></about-intro>

        <about-metamorph></about-metamorph>

        <about-carousel></about-carousel>

        <div class="about__contact">
            <h2>THE CONTACT BUTTON IS RIGHT HERE</h2>

            <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="about__button"><span>LET’S MAKE <br> SOMETHING GREAT
</span></NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    name: 'About',
    components: {
        aboutIntro: () => import('./about/AboutIntro.vue'),
        aboutMetamorph: () => import('./about/AboutMetamorphSection.vue'),
        aboutCarousel: () => import('./about/AboutCarousel.vue'),
    }
}
</script>

<style lang="scss">
@import "@/assets/scss/_mixins.scss";

.about {
    &__intro-wrapper {
        padding-top: 12rem;
    }

    &__title-wrapper {
        text-align: center;
        margin-bottom: 8rem;

        h1 {
            font-family: "Colombo";
            color: $teal;
            font-size: 6.25rem;
            text-transform: uppercase;
        }
    }

    &__large-butterfly {
        display: flex;
        padding-left: 15rem;

        &__text-wrapper {
            width: 55%;
        }

        &__heading {
            font-size: 4rem;
            color: $pink;
            font-family: 'Montserrat';
        }

        &__text {
            color: $white;
            font-size: 2rem;
            font-family: 'MyriadPro';
            padding-top: 2rem;
            width: 100%;
            line-height: 150%;
        }

        &__img {
            width: 100%;
            max-width: 20rem;
            position: absolute;
            left: 80%;
            top: 10rem;
        }
    }

    &__metamorph {
        margin-top: 20rem;
        
        height: 100vh;

        padding-top: 8rem;
        width: 100%;

        &__heading {
            color: $white;
            font-size: 2rem;
            font-family: 'MyriadPro';
            margin-bottom: 3rem;
            text-align: center;
        }

        &__wrapper {
            display: flex;
            mix-blend-mode: lighten;
        }

        &__lists {
            padding: 5rem 0 0 5rem;
        }

        &__pink-heading {
            color: $pink;
            font-size: 1.25rem;
            margin-bottom: 1.5rem;
        }

        &__list {
            margin-bottom: 3rem;

            li {
                counter-increment: item;
                color: $white;
                font-family: 'Montserrat';
                padding-bottom: 1rem;
            }

            li:before {
                margin-right: 10px;
                content: counter(item);
                color: $teal;
                display: inline-block;
                font-weight: bold;
            }
        }
    }

    &__overlapping-headers {
        text-align: center;
        margin: 3rem auto;

        @include overlapping-headers;
    }

    &__carousel-slider {
        background: rgba(0, 0, 0, 0.137);
        color: $white;
        padding: 5rem;

        h2 {
            font-size: 2rem;
            font-family: 'Montserrat';
            color: $pink;
            text-align: center;
            max-width: 28rem;
            margin: 0 auto 2rem;
        }

        p {
            font-size: 1.25rem;
            font-family: 'Montserrat';
            line-height: 150%;
            &:nth-of-type(2) {
                margin-top: 2rem;
            }
        }

        ul {
            margin-bottom: 1rem;
        }

        ul li {
            font-size: 1.25rem;
            font-family: 'Montserrat';
        }
    }

    &__contact {
        display: flex;
        max-width: 960px;
        width: 100%;
        margin: 5rem auto;
        align-items: center;
        justify-content: space-between;

        h2 {
            color: $teal;
            font-family: 'Colombo';
            font-size: 3rem;
            max-width: 60%;
        }
    }

    &__button {
        @include button;
        max-width: 15rem;
        background: rgba(255, 255, 255, 0.25);
        box-shadow: 0 8px 32px 0 rgb(31 38 135 / 37%);
        transition: 0.16s;
    }
    &__button:hover{
        border-image: linear-gradient(-90deg, rgba(22, 255, 255, 0.2) 0%, rgba(255, 24, 247, 0.2) 100%);
        background: linear-gradient(90deg, rgba(22, 255, 255, 0.2) 0%, rgba(255, 24, 247, 0.2) 100%);

    }
}

.VueCarousel-dot {
    padding: 0 !important;
    margin: 0.25rem;
    background-color: transparent !important;
    border: 1px solid #fff !important;
}

.VueCarousel-dot--active {
    background-color: #fff !important;
    border: none !important;
}

@media only screen and (min-width: 768px) and (max-width: 1440px) {
    .about {
        &__intro-wrapper {
            padding-top: 7rem;
        }

        &__large-butterfly {
            padding-left: 7rem;

            &__heading {
                font-size: 3rem;
            }

            &__img {
                max-width: 20rem;
                top: 15rem;
                left: 60%;
            }
        }

        &__title-wrapper {
            margin-bottom: 1rem;
        }

        &__metamorph {
            margin-top: 5rem;
            height: auto;

            &__heading {
                margin: 0;
            }

            &__wrapper {
                align-items: center;

                img {
                    width: 50%;
                    height: 50%;
                }
            }
        }

        &__overlapping-headers {
            h1 {
                font-size: 3.25rem;
            }

            h2 {
                font-size: 3rem;
                top: -1.75rem;
            }
        }

        &__contact {
            padding: 0 2rem;
        }
    }
}

@media only screen and (max-width: 767px) {
    .about {
        padding: 0 0.5rem;

        &__intro-wrapper {
            padding-top: 10rem;

            h1 {
                font-size: 3.5rem;
            }
        }

        &__title-wrapper {
            margin-bottom: 2rem;
        }

        &__large-butterfly {
            padding: 0;

            &__text-wrapper {
                width: 100%;
            }

            &__heading {
                font-size: 2rem;
                text-align: center;
            }

            &__text {
                font-size: 1.25rem;
            }

            &__img {
                max-width: 5rem;
                top:48%;
                right: 0;
                left: 55%;
            }
        }

        &__metamorph {
            margin-top: 5rem;
            height: auto;

            &__heading {
                font-size: 1.75rem;
            }

            &__wrapper {
                display: block;

                img {
                    width: 100%;
                }
            }

            &__lists {
                padding: 0;
            }
        }

        &__overlapping-headers {
            h1 {
                font-size: 1.5rem;
            }
            h2 {
                font-size: 1.25rem;
                top: 0;
             
            }
        }

        &__carousel-slider {
            padding: 1rem;

            ul li {
                padding: 1rem 0;

                &:nth-child(even) {
                    padding: 0;
                }
            }
        }

        &__contact {
            flex-direction: column;

            h2 {
                max-width: 100%;
                font-size: 2rem;
                text-align: center;
                margin-bottom: 1rem;
            }
        }
    }
}

</style>