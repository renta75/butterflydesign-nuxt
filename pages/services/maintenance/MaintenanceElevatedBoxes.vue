<template>
    <div class="container maintenance__elevated-boxes">
        <div class="maintenance__elevated-boxes__wrapper">
            <div>
                <h3 class="maintenance__elevated-boxes__heading">STARTER PLAN</h3>
                <h5 class="maintenance__elevated-boxes__price">€ <span>40</span>/month</h5>
                <ul class="maintenance__main-section__list">
                    <li class="maintenance__main-section__list-item">Core updates</li>
                    <li class="maintenance__main-section__list-item">Monthly site & database backups</li>
                    <li class="maintenance__main-section__list-item">Website restore when down</li>
                    <li class="maintenance__main-section__list-item">Spam comments cleanup</li>
                    <li class="maintenance__main-section__list-item">Performance check</li>
                    <li class="maintenance__main-section__list-item">Security monitoring</li>
                    <li class="maintenance__main-section__list-item">Weekly plugins & themes updates</li>
                    <li class="maintenance__main-section__list-item">Monthly report</li>
                    <li class="maintenance__main-section__list-item">Chat & email support</li>
                    <li class="maintenance__main-section__list-item">Site uptime monitoring</li>
                    <li class="maintenance__main-section__list-item">Content updates and support</li>
                    <li class="maintenance__main-section__list-item">Plugin & theme install</li>
                    <li class="maintenance__main-section__list-item">Performance caching</li>
                    <li class="maintenance__main-section__list-item">SSL Certificate</li>
                    <li class="maintenance__main-section__list-item">No contract - Cancel anytime</li>
                </ul>
                <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="maintenance__elevated-boxes__button starter"><span>Starter Plan</span></NuxtLink>
            </div>
            <div class="maintenance__elevated-boxes__elevated-box">
                <h3 class="maintenance__elevated-boxes__heading">BASIC PLAN</h3>
                <h5 class="maintenance__elevated-boxes__price">€ <span>65</span>/month</h5>
                <ul class="maintenance__main-section__list">
                    <li class="maintenance__main-section__list-item">Core updates</li>
                    <li class="maintenance__main-section__list-item">Monthly site & database backups</li>
                    <li class="maintenance__main-section__list-item">Website restore when down</li>
                    <li class="maintenance__main-section__list-item">Spam comments cleanup</li>
                    <li class="maintenance__main-section__list-item">Performance check</li>
                    <li class="maintenance__main-section__list-item">Security monitoring</li>
                    <li class="maintenance__main-section__list-item">Weekly plugins & themes updates</li>
                    <li class="maintenance__main-section__list-item">Monthly report</li>
                    <li class="maintenance__main-section__list-item">Chat & email support</li>
                    <li class="maintenance__main-section__list-item">Site uptime monitoring</li>
                    <li class="maintenance__main-section__list-item">Content updates and support</li>
                    <li class="maintenance__main-section__list-item">Plugin & theme install</li>
                    <li class="maintenance__main-section__list-item">Performance caching</li>
                    <li class="maintenance__main-section__list-item">SSL Certificate</li>
                    <li class="maintenance__main-section__list-item">No contract - Cancel anytime</li>
                </ul>
                <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="maintenance__elevated-boxes__button basic"><span>BASIC PLAN</span></NuxtLink>
            </div>
            <div>
                <h3 class="maintenance__elevated-boxes__heading">PRO PLAN</h3>
                <h5 class="maintenance__elevated-boxes__price">€ <span>95</span>/month</h5>
                <ul class="maintenance__main-section__list">
                    <li class="maintenance__main-section__list-item">Core updates</li>
                    <li class="maintenance__main-section__list-item">Monthly site & database backups</li>
                    <li class="maintenance__main-section__list-item">Website restore when down</li>
                    <li class="maintenance__main-section__list-item">Spam comments cleanup</li>
                    <li class="maintenance__main-section__list-item">Performance check</li>
                    <li class="maintenance__main-section__list-item">Security monitoring</li>
                    <li class="maintenance__main-section__list-item">Weekly plugins & themes updates</li>
                    <li class="maintenance__main-section__list-item">Monthly report</li>
                    <li class="maintenance__main-section__list-item">Chat & email support</li>
                    <li class="maintenance__main-section__list-item">Site uptime monitoring</li>
                    <li class="maintenance__main-section__list-item">Content updates and support</li>
                    <li class="maintenance__main-section__list-item">Plugin & theme install</li>
                    <li class="maintenance__main-section__list-item">Performance caching</li>
                    <li class="maintenance__main-section__list-item">SSL Certificate</li>
                    <li class="maintenance__main-section__list-item">No contract - Cancel anytime</li>
                </ul>
                <NuxtLink :to="{ path: '/contact', hash: '#contact_form_anchor' }" class="maintenance__elevated-boxes__button pro"><span>PRO PLAN</span></NuxtLink>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MaintenanceElevatedBoxes'
}
</script>