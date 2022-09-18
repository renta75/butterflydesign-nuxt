<template>
  <div class="contact-form">
    <h2 class="contact-form__heading" id="contact_form_anchor">
      How can we help?
    </h2>

    <div class="contact-form__wrapper">
      <div class="contact-form__frm-wrapper">
        <form action="#">
          <input type="text" placeholder="Your appreciated name" />
          <input type="text" placeholder="Your@awesome.email" />
          <textarea
            name=""
            id=""
            cols="30"
            rows="10"
            placeholder="Your finest message"
          ></textarea>
        </form>

        <NuxtLink
          :to="{ path: '/contact', hash: '#contact_form_anchor' }"
          class="contact-form__button"
          ><span>Contact us</span></NuxtLink
        >
      </div>
      <div class="contact-form__info">
        <h3 class="contact-form__info__heading plavo">
          You’ve got questions, we’ve got answers
        </h3>
        <p class="contact-form__info__text">Open weekdays: 9am - 5pm</p>
        <h3 class="contact-form__info__heading">Let’s talk?</h3>
        <h3 class="contact-form__info__heading">
          Share your excitement with us.
        </h3>
        <p class="contact-form__info__text">
          You can also check us out and follow us on social media
        </p>

        <div class="contact-form__icons">
          <img src="@/assets/contact/Icon-Facebook.svg" alt="" />
          <img src="@/assets/contact/Icon-Instagram.svg" alt="" />
          <img src="@/assets/contact/Icon-Telegram.svg" alt="" />
          <img src="@/assets/contact/Icon-Twitter.svg" alt="" />
          <img src="@/assets/contact/Icon-Youtube.svg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
.plavo{
	color:#16ffff !important;
}
.contact-form {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  height: 70vh;

  &__heading {
    font-size: 2rem;
    color: $white;
    margin-bottom: 5rem;
    text-align: center;
  }

  &__frm-wrapper,
  &__info {
    width: 50%;
  }

  &__wrapper {
    display: flex;

    input,
    textarea {
      display: block;
      width: 75%;
      background: #231051;
      box-shadow: none;
      border: none;
      border-radius: 3px;
      color: white;
      font-family: "Montserrat", sans-serif;
      resize: none;
    }

    input {
      height: 3rem;
      margin-bottom: 1rem;
      padding: 1rem;
      color: white;
    }

    textarea {
      padding: 1rem;
    }

    ::placeholder {
      color: #fff;
    }
  }

  &__info {
    &__heading {
      width: 75%;
      font-size: 1.5rem;
      color: $pink;
      font-family: "Montserrat";
    }

    &__text {
      color: $white;
      font-family: "MyriadPro";
      padding: 2rem 0;
    }
  }

  &__button {
    @include button;
    max-width: 28rem;
    margin: 2rem 0;
    background: rgba(255, 255, 255, 0.25);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    backdrop-filter: blur(4px);
    -webkit-backdrop-filter: blur(4px);
    border-radius: 10px;
	transition: 0.16s;
    border: 1px solid rgba(255, 255, 255, 0.18);
  }
  &__button:hover {
	border-width: 1px;
	border-style: solid;
	border-image: linear-gradient(-90deg, rgba(22, 255, 255, 0.2) 0%, rgba(255, 24, 247, 0.2) 100%);
	background: linear-gradient(90deg, rgba(22, 255, 255, 0.2) 0%, rgba(255, 24, 247, 0.2) 100%);
  }
  &__icons {
    display: flex;

    img {
      max-width: 2rem;
      margin-right: 1rem;
      width: 100%;
      height: 100%;
    }
  }
}

@media only screen and (min-width: 1024px) and (max-width: 1440px) {
  .contact-form {
    &__button {
      width: 75%;
    }
  }
}

@media only screen and (min-width: 768px) and (max-width: 1023px) {
  .contact-form {
    height: auto;

    &__button {
      width: 75%;
    }
  }
}

@media only screen and (max-width: 767px) {
  .contact-form {
    height: auto;
    padding: 0 0.5rem;

    &__wrapper {
      flex-direction: column;

      input,
      textarea {
        width: 100%;
      }
    }

    &__frm-wrapper,
    &__info {
      width: 100%;
      text-align: center;
    }

    &__info {
      &__heading {
        width: 100%;
      }
    }

    &__button {
      margin: 2rem auto;
    }
    &__icons {
      display: flex;
      justify-content: center;

      img {
        max-width: 2rem;
        margin-right: 1rem;
        width: 100%;
        height: 100%;
      }
    }
  }
}
</style>
