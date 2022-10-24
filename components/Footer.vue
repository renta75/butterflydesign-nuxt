
<template>
	<nav class="footer">
		<div class="container footer__wrapper">
            <div class="footer__logo-wrapper">
                <img alt="Logo" src="@/assets/footer-logo.svg" class="footer__logo" width="">
                <span class="footer__text">contact@butterflydesign.hr</span>
                <span class="footer__text">Senjska 125, HR-47303 Josipdol, Croatia</span>
                <span class="footer__text">+385914777020</span>
            </div>

            <div class="footer__services-wrapper">
                <h3 class="footer__services-heading">Services</h3>
                <NuxtLink to="/services/web-development" class="footer__text"><span>Web development</span></NuxtLink>
                <NuxtLink to="/services/e-commerce" class="footer__text"><span>E-commerce</span></NuxtLink>
                <NuxtLink to="/services/maintenance" class="footer__text"><span>Maintenance</span></NuxtLink>
                <NuxtLink to="/services/graphic-design" class="footer__text"><span>Graphic design</span></NuxtLink>
            </div>

            <div class="footer__newsletter-wrapper">
                <h3 class="footer__services-heading">Newsletter</h3>
                <p class="footer__text">Subscribe for new and great deals</p>

                <div class="footer__newsletter-field">
                    <input type="text" placeholder="your@awesome.email">
                    <div class="footer__button"><span>GO</span></div>
                </div>
            </div>
            
            <div class="footer__resources-wrapper removeable">
                <h3 class="footer__services-heading">Resources</h3>
                <span class="footer__text">FAQ</span>
                <span class="footer__text">Privacy Policy</span>
                <span class="footer__text">Terms and Conditions</span>
            </div>

           
        </div>
        <div class="footer__icons">
            <img src="@/assets/contact/Icon-Facebook.svg" alt="">
            <img src="@/assets/contact/Icon-Instagram.svg" alt="">
            <img src="@/assets/contact/Icon-Telegram.svg" alt="">
            <img src="@/assets/contact/Icon-Twitter.svg" alt="">
            <img src="@/assets/contact/Icon-Youtube.svg" alt="">
        </div>
        <p class="footer__copy">&copy; 2022 Butterfly Design LLC</p>
	</nav>
</template>


<script>
  export default {
    scrollToTop: true
  }
</script>
<style lang="scss">
    @import '@/assets/scss/_variables.scss';
    @import '@/assets/scss/_mixins.scss';
    
    .footer {
        background: #130037;
        margin-top: 5rem;

        min-height: calc(100vh - 100px)
        &__logo {
            width: 100%;
            height: 100%;
            max-height: 8rem;
            max-width: 12rem;
            padding-top: 1rem;
        }
    
        &__wrapper {
            display: flex;
            justify-content: space-between;
        }
    
        &__services-heading {
            color: #ff18f7;
            font-family: 'Colombo';
            font-size: 1.25rem;
            text-transform: uppercase;
            margin: 3rem 0 1rem;
        }
    
        &__text {
            color: $white;
            display: block;
            padding: .25rem 0;
            text-decoration: none;
            transition: 0.16s;
        }
        &__text:hover {
            color: #16ffff;
            cursor: pointer;
        }
    
        &__newsletter-field {
            display: flex;
        }
    
        input {
            flex: 0 0 75%;
            background: #231051;
            color: white;
            box-shadow: none;
            border: none;
            border-radius: 6px;
            margin-top: .25rem;
            margin-bottom: 1rem;
            padding: .5rem;
        }
    
        ::placeholder {
            color: white;
        }
    
        &__button {
            @include button;
            height: 2rem;
            border-radius: 6px;
            padding: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-top: .25rem;
        }
    
        &__icons {
            display: flex;
            justify-content: center;
            padding-top: 2rem;
    
            img {
                width: 100%;
                height: 100%;
                max-width: 2rem;
                margin-right: 1rem;
            }
        }
    
        &__copy {
            text-align: center;
            color: $white;
            padding: 2rem 0;
        }
    }
    @media only screen and (max-width: 767px) {
        .footer {
            &__wrapper {
                display: none;
            }
        }
    }
    .removeable{
       opacity: 0;
       visibility: hidden;
    }
    </style>

