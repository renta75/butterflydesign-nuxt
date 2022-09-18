<template>
  <div class="e-commerce">

    <ecommerce-intro></ecommerce-intro>

    <ecommerce-elevated-boxes></ecommerce-elevated-boxes>

    <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="e-commerce__button"><span>Contact us</span></NuxtLink>

    <ecommerce-accordions></ecommerce-accordions>

    <ecommerce-inline-boxes></ecommerce-inline-boxes>

    <ecommerce-store-features></ecommerce-store-features>

    

    <ecommerce-other-services></ecommerce-other-services>
  </div>
</template>

<script>
export default {
  name: 'ECommerce',
  components: {
      ecommerceIntro: () => import('./EcommerceIntro.vue'),
      ecommerceElevatedBoxes: () => import('./EcommerceElevatedBoxes.vue'),
      ecommerceAccordions: () => import('./EcommerceAccordions.vue'),
      ecommerceInlineBoxes: () => import('./EcommerceInlineBoxes.vue'),
      ecommerceStoreFeatures: () => import('./EcommerceStoreFeatures.vue'),
      ecommerceOtherServices: () => import('./EcommerceOtherServices.vue'),
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_mixins.scss';

.e-commerce {
    &__intro {
        @include service-page-intro;
        height: 100vh;
        padding-top: 8rem;

        .container {
            display: flex;
        }

        video {
            width: 50%;
            position: relative;
            top: -3rem;
            mix-blend-mode: lighten;
            opacity: 0.8;
        }

        &__text-wrapper {
            width: 50%;
            margin: 8rem 0 0 1rem;
        }
        &__text{
            line-height: 190%;
        }

        &__subheading {
            font-size: 4rem;
            color: $pink;
            font-family: 'Montserrat';
            margin: 2rem 0;
        }
    }

    &__elevated-boxes {
        position: relative;
        border-radius: 5px;
        @include elevated-boxes;

        &__wrapper {
            h3 {
                padding-top: 0;
            }
        }

        .first-img {
            max-width: 3rem;
        }

        &__elevated-box {
            top: -0.5rem;
            height: 21rem;
        }

        &__regular-img {
            max-width: 8rem;
        }
        p{
            line-height: 120%;
        }
    }

    &__button {
        @include button;
        opacity: 0;
        margin: 5rem auto;
    }
}


.section-accordions {
    &__wrapper {
        display: flex;
        justify-content: center;
    }

    &__heading {
        font-size: 4rem;
        color: $pink;
        text-align: center;
        margin-bottom: 4rem;
    }

    .vsa-list {
        background-color: transparent;
        border: none;
        padding-top: 3rem;
    }

    .vsa-item {
        &--is-active &__heading, &:not(:last-of-type) {
            border: none;
        }

        &__trigger {
            color: $teal;

            &:hover, &:focus {
                color: $pink;
                background-color: transparent;
            }

            &__icon--is-default:before, &__icon--is-default:after {
                background-color: $pink;
            }
        }

        &__content {
            color: $white;
            line-height: 150%;
        }
    }

    &__image {
        max-width: 35rem;
        margin: 0 auto;
        display: block;
    }
}

.inline-boxes {
    display: flex;

    &__box {
        text-align: center;

        box-shadow: 5px 5px 30px rgba(0, 0, 0, 0.5);
        border-radius: 15px;
        flex: 0 0 25%;
        margin: 0 0.5rem;
        height: 28.75rem;
        position: relative;
    }

    &__image {
        max-width: 8rem;
        position: absolute;
        top: -4rem;
        left: 50%;
        transform: translateX(-50%);
    }

    &__heading {
        color: #16FFFF;
        text-transform: uppercase;
        font-size: 1.25rem;
        margin-top: 7rem;
        margin-bottom: 2rem;
    }

    &__text {
        color: $white;
        padding: 0 2rem;
        line-height: 190%;
    }
}

.ecommerce {
    &__bottom-section {
        &__h2 {
            color: $white;
            text-align: center;
            font-size: 2.25rem;
            margin-top: 5rem;
        }

        &__list-wrapper {
            display: flex;
            justify-content: center;
            margin: 0 auto;
        }

        &__list {
            padding: 3rem;
        }

        &__list-item {
            color: $white;
            padding: 0.5rem 0;

            &::before {
                content: '';
                display: inline-block;
                margin-right: 0.5rem;
                height: 1rem;
                width: 1rem;
                background-size: 1rem 1rem;
                background-image: url('~@/assets/Icon-Kvacica.svg');
                background-repeat: no-repeat;
            }
        }

        &__button {
            @include button;

            margin: 0 auto;
            max-width: 12rem;
        }

        &__other-services-h2 {
            @include styled-heading;
        }

        &__other-services-wrapper {
            display: flex;
            justify-content: space-between;
            max-width: 45rem;
            margin: 0 auto;
        }

        &__other-service {
            text-align: center;
            text-decoration: none;

            img {
                max-width: 5rem;
                height: 5.5rem;
            }
        }

        &__other-service-heading {
            color: white;
            display: block;
            text-decoration: none;
        }
    }
}

@media only screen and (min-width: 1024px) and (max-width: 1440px) {
    .e-commerce {
        &__intro {
            &__heading {
                font-size: 5rem;
            }
            &__subheading {
                font-size: 4rem;
            }
        }
    }
    .inline-boxes {
        &__box {
            flex: 0 0 23.5%;
        }
    }
}

@media only screen and (min-width: 768px) and (max-width: 1023px) {
    .e-commerce {
        &__intro {
            padding-top: 5rem;

            &__heading {
                font-size: 3.75rem;
            }

            &__subheading {
                font-size: 3rem;
            }
        }

        &__main-section {
            &__img {
                padding: 3rem;
            }
        }

        &__elevated-boxes {
            &__wrapper {
                max-height: 24rem;
            }
            &__elevated-box {
                height: 25rem;
            }
        }
    }

    .section-accordions {
        height: 100vh;

        &__heading {
            font-size: 3rem;
        }
        &__image {
            max-width: 25rem;
        }
    }

    .inline-boxes {
        flex-wrap: wrap;

        &__box {
            flex: 0 0 45%;
            margin: 1rem;
        }
        &__image {
            position: static;
            transform: none;
            height: auto;
            margin-top: 1rem;
        }
        &__heading {
            margin-top: 1rem;
        }
    }
}

@media only screen and (max-width: 767px) {
    .e-commerce {
        padding: 0;

        &__intro {
            height: auto;

            .container {
                flex-direction: column;
            }
            &__text-wrapper {
                margin: 0;
                width: 100%;
                text-align: center;
            }
            &__heading {
                font-size: 3rem;
            }
            &__subheading {
                font-size: 2rem;
            }
            video {
                width: 100%;
            }
        }

        &__elevated-boxes {
            &__wrapper {
                flex-direction: column;
                max-height: none;
            }
        }

        .section-accordions {
            &__wrapper {
                flex-direction: column-reverse;
            }
            &__heading {
                font-size: 2.5rem;
            }
            .vsa-item__trigger__content {
                text-align: left;
            }
        }

        .inline-boxes {
            flex-direction: column;
            margin-top: 5rem;

            &__box {
                height: 25rem;
                flex: auto;
                margin: 1rem;
            }
            &__image {
                margin: 1rem 0;
                position: relative;
                top: 0;
                left: 0;
                transform: none;
            }
            &__heading {
                margin: 0;
            }
            &__text {
                padding: 2rem;
            }
        }

        .ecommerce {
            &__bottom-section {
                &__list-wrapper {
                    flex-direction: column;
                    padding: 2rem 0;
                }
                &__list {
                    padding: 0;
                }
                &__other-services-h2 {
                    &:before, &:after {
                        display: none;
                    }
                }
                &__other-service-heading {
                    font-size: 0.75rem;
                }
            }
        }
    }
}

</style>