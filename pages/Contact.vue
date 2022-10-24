<template>
  <div class="contact">
    <div class="container contact__intro-wrapper">
        <div class="contact__title-wrapper">
            <h1 class="contact__h1 animate__animated animate__fadeInLeft">CONTACT US</h1>
        </div>
    </div>

    <div class="container contact__contact-info">
        <div class="contact__contact-info__letsmeet">
            <img src="@/assets/contact/LetsMeet.png" alt="" class="contact__contact-info__image">
            <h3 class="contact__contact-info__heading">LETS MEET  VISIT US</h3>
            <p class="contact__contact-info__text">Trnjanska cesta 63, HR-10000 Zagreb, Croatia</p>
 
        </div>
        <div class="contact__contact-info__hireus">
            <img src="@/assets/contact/HireUs.png" alt="" class="contact__contact-info__image">
            <h3 class="contact__contact-info__heading">HIRE US!  LET’S TALK</h3>
<p class="contact__contact-info__text">Ready to bring your product to life? We are too</p>
        </div>
        <div class="contact__contact-info__creative">
            <img src="@/assets/contact/Creative.png" alt="" class="contact__contact-info__image image-position">
            <h3 class="contact__contact-info__heading">CREATIVE? WANT TO JOIN US?</h3>
            <p class="contact__contact-info__text">Think you got what it takes? Hit us up!</p>
        </div>
    </div>

    <contact-form></contact-form>
  </div>
</template>

<script>
import contactForm from '@/components/ContactForm.vue';

export default {
    components: {
        contactForm
    }
}
</script>

<style lang="scss">
@import '@/assets/scss/_mixins.scss';

.contact {
    &__intro-wrapper {
        padding-top: 12rem;
    }

    &__title-wrapper {
        text-align: center;
        margin-bottom: 8rem;

        h1 {
            font-family: 'Colombo';
            color: $teal;
            font-size: 6.25rem;
            text-transform: uppercase;
        }
    }

    &__contact-info {
        display: flex;
        text-align: center;

        div {
            flex: 0 0 33.33333%;
            padding: 0 8rem 7rem;
        }

        .image-position {
            margin: 1rem 0 0.25rem;
        }

        &__heading {
            color: $teal;
            font-family: 'Colombo';
            font-size: 2rem;
            margin: 1rem 0;
        }

        &__text {
            color: $white;
            margin-bottom: 1rem;
        }

        &__pink {
            color: $pink;
            font-size: 1.25rem;
            margin-top: 35px;
        }
    }
}


@media only screen and (min-width: 1024px) and (max-width: 1440px) {
    .contact {
        &__contact-info {
            div {
                padding: 0 3rem 5rem;
            }
        }
    }
}

@media only screen and (min-width: 768px) and (max-width: 1023px) {
    .contact {
        padding: 0 0.5rem;

        &__intro-wrapper {
            padding-top: 7rem;
        }

        &__heading {
            margin: 5rem 0;
        }

        &__contact-info {
            div {
                padding: 0.5rem;
            }
        }
    }
}

@media only screen and (max-width: 767px) {
    .contact {
        &__intro-wrapper {
            padding-top: 10rem;
        }

        &__title-wrapper {
            margin-bottom: 5rem;

            h1 {
                font-size: 3rem;
            }
        }

        &__contact-info {
            flex-direction: column;

            div {
                flex: 1 1 auto;
                padding: 3rem 2rem;
            }
        }
    }
}
.telefon-kontakt{
    text-decoration: none;
    color: #ff18f7;
}
</style>