<template>
  <div class="maintenance">

    <maintenance-intro></maintenance-intro>

    <div class="maintenance__main-section">

        <maintenance-images></maintenance-images>

        <h2 class="maintenance__main-section__other-services-h2">Pick the perfect plan for your business</h2>

        <maintenance-elevated-boxes></maintenance-elevated-boxes>

        <maintenance-other-services></maintenance-other-services>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Maintenance',
  components: {
      maintenanceIntro: () => import('./MaintenanceIntro.vue'),
      maintenanceImages: () => import('./MaintenanceImages.vue'),
      maintenanceElevatedBoxes: () => import('./MaintenanceElevatedBoxes.vue'),
      maintenanceOtherServices: () => import('./MaintenanceOtherServices.vue'),
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_mixins.scss';

.maintenance {
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

        &__subheading {
            font-size: 3rem;
            color: $pink;
            font-family: 'Montserrat';
            margin: 1rem 0 2rem;
        }

        &__text {
            width: 75%;
            line-height: 200%;
        }
        &__other-service-heading {
    color: white;
}
    }

    &__elevated-boxes {
        position: relative;
        border-radius: 5px;
        @include elevated-boxes;

        &__wrapper {
            max-height: 55rem;

            div {
                flex: 0 0 33.333333%;
            }

            h3 {
                padding-top: 0;
            }
        }

        &__elevated-box {
            top: -0.5rem;
            height: 56rem;
        }

        &__heading {
            margin-top: 3rem;
        }

        &__price {
            color: $pink;
            margin-top: 2rem;

            span {
                font-size: 3rem;
                font-family: 'Colombo'
            }
        }

    &__button {
        @include button;
        max-width: 15rem;
        font-size: 1rem;
        margin: 0 auto;
        background: rgba(255, 255, 255, 0.25);
        box-shadow: 0 8px 32px 0 rgb(31 38 135 / 37%);
        transition: 0.16s;
    }
    .starter{
        background: #16FFFF;
        color:black;
    }
    .basic{
         background: linear-gradient(90deg, rgba(22, 255, 255, 0.758) 0%, rgb(255, 24, 247) 100%);
        color:rgb(255, 255, 255);
    }
    .pro{
        background: #FF24FF;
        color:rgb(255, 255, 255);
    }
    .starter:hover{
        background: #16ffff72;
        color: white;
    }
    .basic:hover{
        background: linear-gradient(90deg, rgba(22, 255, 255, 0.488) 0%, rgba(255, 24, 247, 0.46) 100%);
        color:rgb(255, 255, 255);
    }
    .pro:hover{
        background: #ff24ff72;
        color: white;
    
    }
}


    &__main-section {
        width: 100%;
        max-width: 960px;
        margin: 0 auto;
        text-align: center;

        &__heading {
            font-family: 'Montserrat';
            color: $pink;
            font-size: 4rem;
            padding: 2rem 0;
        }

        &__subheading {
            font-family: 'Montserrat';
            color: $white;
            padding-bottom: 5rem;
        }

        &__images-wrapper {
            display: flex;
            flex-wrap: wrap;
            margin: 5rem 0;
        }

        &__img {
            width: 30%;
            flex: 0 0 33.333333%;
            padding: 1rem;
            transition: 0.2s ease-in-out;

            img {
                width: 100%;
                max-width: 6rem;
            }
        }
        &__img:hover{
            background: #ff18f723;
        }

        &__text {
            color: $white;
            margin: 2rem 0 4rem;
            line-height: 200%;
        }

        &__h3 {
            color: $pink;
            padding-top: 2rem;
            font-size: 1.25rem;
        }

        &__h2 {
            color: $white;
            text-align: center;
            font-size: 2.25rem;
        }

        &__list-wrapper {
            display: flex;
            justify-content: center;
            margin: 0 auto;
        }

        &__list {
            padding: 2rem;
            text-align: left;
            line-height: 110%;
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
            text-decoration: none;

            img {
                max-width: 5rem;
                height: 5.5rem;
            }
        }

        &__other-service-heading {
            color: $white;
            display: block;
            text-decoration: none;
        }
    }
}

@media only screen and (min-width: 1024px) and (max-width: 1440px) {
    .maintenance {
        &__intro {
            &__heading {
                font-size: 5rem;
            }
            &__subheading {
                font-size: 4rem;
            }
        }
    }
}

@media only screen and (min-width: 768px) and (max-width: 1023px) {
    .maintenance {
        &__intro {
            padding-top: 5rem;

            &__heading {
                font-size: 3.75rem;
            }

            &__subheading {
                font-size: 3rem;
            }
        }
        &__elevated-boxes {
            &__wrapper {
                max-height: 60rem;
            }
            &__elevated-box {
                height: 61rem;
            }
        }
    }
}


@media only screen and (max-width: 767px) {
    .maintenance {
        padding: 0 0.5rem;

        &__intro {
            .container {
                flex-direction: column;
            }
            video {
                width: 100%;
                top: 0;
            }
            &__text-wrapper {
                width: 100%;
                margin: 0;
                text-align: center;
            }
            &__heading {
                font-size: 2.5rem;
            }
            &__subheading {
                font-size: 2rem;
                width: 100%;
            }
            &__text {
                width: 100%;
            }
        }

        &__main-section {
            &__img {
                width: 100%;
                flex: 1 1 auto;
                padding: 0 2rem;
            }

            &__other-services-h2 {
                &:before, &:after {
                    display: none;
                }
            }

            &__other-service-heading {
                font-size: 0.75rem;
                color: white;
            }
        }

        &__elevated-boxes {
            ::after {
                display: none;
            }

            &__wrapper {
                flex-direction: column;
                max-height: fit-content;

                div {
                    flex: 1 1 auto;
                    border: 2px solid $teal;
                }
            }

            &__elevated-box {
                height: auto;
                top: 0;
                margin: 1rem 0;
            }

            &__button {
                margin: 2rem auto;
            }
        }
    }
}

</style>