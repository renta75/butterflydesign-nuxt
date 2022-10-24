<template>
    <div>
        <div class="container about__overlapping-headers">
            <h1 class="about__overlapping-headers-h1">www.butterfly.design</h1>
            <h2 class="about__overlapping-headers-h2">THE GLOVE IN THE DARK</h2>
        </div>

        <carousel :per-page="1" :mouse-drag="false">
            <slide>
                <div class="container about__carousel-slider">
                    <h2>WHERE WE CAME FROM</h2>
                    <p>
                      Butterfly Design was born in a beautiful European country called Croatia. A small place with worldwide recognition for its natural beauty and the striking Adriatic Sea. This was the starting point that inspired us to take inspiration from art made by nature, just like butterflies. Nature creates extraordinary beings that combine beauty and functionality just as we combine those elements in every digital product we create.
</p>
                </div>
            </slide>
            <slide>
                <div class="container about__carousel-slider">
                    <h2>VALUES</h2>
                    <p>
                        We believe in productivity driven by a positive attitude. That means that we like to make our work environment as positive as humanly possible by putting a smile on our client’s faces and celebrating every success along the way with them.

                    </p>

                    <p>Beliefs:</p>
                    <ul>
                        <li>- Looking at our client as an individual first, and as a business second</li>
                        <li>- Having contagious enthusiasm about every new project</li>
                        <li>- Bringing together innovative technology and user psychology</li>
                    </ul>
                </div>
            </slide>
        </carousel>
    </div>
</template>

<script>
export default {
    name: 'AboutCarousel'
}
</script>