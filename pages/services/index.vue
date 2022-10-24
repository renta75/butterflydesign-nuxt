<template>
  <div class="services">
    <div class="container services-intro__wrapper">
        <div class="services-intro__title-wrapper">
            <h1 class="services-intro__h1">SERVICES THAT LAUNCH</h1>
            <h2 class="services-intro__h2 animate__animated animate__backInLeft">YOUR BUSINESS ABOVE THE COMPETITION</h2>
        </div>
    </div>

    <services-boxes></services-boxes>

    <services-why-us></services-why-us>
  </div>
</template>

<script>
export default {
    name: 'Services',
    components: {
        servicesWhyUs: () => import('./ServicesWhyUs.vue'),
        servicesBoxes: () => import('./ServicesBoxes.vue'),
    }
}
</script>

<style lang="scss">
@import '@/assets/scss/_mixins.scss';
.rozo{
    color: $pink;
}
.services {
    .services-intro {
        &__title-wrapper {
            text-align: center;
            padding: 12rem 0 8rem;
            @include overlapping-headers;
        }
    }

    &__wrapper {
        display: flex;
		justify-content: space-between;
    }

    .services-wrapper {
		display: flex;
		justify-content: space-between;

        &__box {
            box-shadow: 0 0 20px #000;
            margin: 0 .5rem;
            padding: 2rem;
            text-align: center;
            position: relative;
        }
        &__top-img {
            position: absolute;
            width: 8rem;
            top: -5rem;
            left: 50%;
            transform: translateX(-50%);
        }

        &__heading {
            color: $pink;
            text-transform: uppercase;
            font-size: 1.5rem;
            padding: 3rem 0;
            font-family: 'Montserrat';
        }

        &__text {
            color: $white;
            font-family: 'Montserrat';
            line-height: 150%;
        }

        &__link {
            display: block;
            color: #16ffff;
            text-decoration: none;
            text-transform: uppercase;
            padding-top: 2rem;
            font-family: 'Montserrat';
        }
    }
}

.services-why-us-headings {
    text-align: center;
    display: block;

    &__h2 {
        font-size: 3rem;
        font-family: 'Montserrat';
        color: $white;
        padding: 5rem 0 0;
    }

    &__h3 {
        font-size: 1.5rem;
        font-family: 'Montserrat';
        color: $white;
        padding: 2rem 0 5rem;
    }
}

.services-why-us {
	&__services-why-us-wrapper {
		position: relative;
		text-align: center;
		z-index: 10;
		margin-top: 3rem;
		flex-direction: column;
	}
	&__title-wrapper {
		@include overlapping-headers;
	}
	&__services-why-us-content-wrapper {
		position: relative;
		margin-bottom: 10rem;
	}
	&__box-wrapper {
		width: 100%;
	}
	&__box-wrapper-row {
		display: flex;
		justify-content: space-between;
		width: 100%;
	}
	&__box-wrapper-row:nth-child(even) {
		margin-top: 1rem;
	}
	&__box {
		display: flex;
		flex-direction: column;
		justify-content: center;
		text-align: center;
		width: 50%;
		height: 20rem;
		padding: 0 10rem;
	}
	&__box:nth-child(odd) {
		background: rgba(0, 0, 0, 0.137);
		mix-blend-mode: normal;
	}
	&__box:nth-child(even) {
		margin-left: 1rem;
		background: rgba(0, 0, 0, 0.137);
	}
	&__box-heading {
		font-size: 1.75rem;
		margin-bottom: 2rem;
		color: $pink;
		text-transform: uppercase;
		font-family: 'Montserrat';
	}
	&__box-text {
		color: $white;
        line-height: 130%;
		font-family: 'Montserrat';
	}
	&__buttons {
		display: flex;
		justify-content: space-around;
		margin: 5rem auto;
		max-width: 1440px;
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

.services-technologies {
	text-align: center;

	&__h2 {
		font-size: 1.5rem;
		color: $white;
		margin: 3rem 0;
	}
	&__tech {
		display: flex;
		justify-content: space-between;
		padding: 0 12rem;
		margin-bottom: 5rem;

		img {
			width: auto;
			max-height: 8rem;
		}
	}
}



@media only screen and (min-width: 1024px) and (max-width: 1440px) {
    .services-why-us {
        &__box {
            padding: 0 2rem;
        }
    }
}

@media only screen and (min-width: 768px) and (max-width: 1023px) {
    .services {
        padding: 0 0.5rem;

        .services-intro {
            &__title-wrapper {
                padding: 9rem 0 5rem;

                h1 {
                    font-size: 4rem;
                }
                h2 {
                    font-size: 3.5rem;
                    top: -2rem;
                }
            }
        }

        .services-wrapper {
            flex-wrap: wrap;
            justify-content: center;

            &__box {
                flex: 0 0 45%;
                margin: 1rem;
            }

            &__top-img {
                position: relative;
                top: 0;
                left: 0;
                transform: none;
            }

            &__heading {
                padding: 1.5rem 0;
            }
        }

        .services-why-us {
            &__box {
                padding: 1rem;
            }
        }

        .services-technologies {
            &__tech {
                padding: 0;
            }
        }
    }
}

@media only screen and (max-width: 767px) {
    .services {
        .services-wrapper {
            flex-direction: column;

            &__box {
                margin-bottom: 8rem;
            }
        }
        .services-intro {
            &__title-wrapper {
                h1 {
                    font-size: 3rem;
                }
                h2 {
                    font-size: 2.25rem;
                    top: -20px;
                }
            }
        }
        .services-why-us {
            &__box-wrapper-row {
                flex-direction: column;
                margin: 0;
            }
            &__box {
                width: 100%;
                height: auto;
                padding: 1.5rem;
                margin: 1rem 0 0;
            }
            &__button {
                font-size: 1rem;
                max-width: 10rem;
            }
        }
        .services-technologies {
            &__tech {
                display: block;
                padding: 0;

                img {
                    margin: 1rem;
                }
            }
        }
    }
 
}

</style>