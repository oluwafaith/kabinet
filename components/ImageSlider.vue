<template>
    <div>
        <VueSlickCarousel v-bind="settings">
        <div class="h-screen w-96 bg-gradient-to-b from-sky-900 to-sky-600 text-white">
            <div class="flex justify-between h-full px-32">
                <div class="self-end pb-32">
                    <h1 class="text-6xl font-semibold mb-6">Influence the change</h1>
                    <h1 class="text-6xl font-semibold mb-6">you want to see</h1>
                    <p class="mb-12">“The most important political office is that of <br />the private citizen.”</p>
                    <p class="mb-6">– Louis D. Brandeis</p>
                    <nuxt-link to="/events">
                        <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-0">Find Events</a>
                    </nuxt-link>
                </div>
                <img class="self-end w-96" src="/guy1.png" alt="">
            </div>
        </div>
        <div class="h-screen w-96 bg-gradient-to-b from-sky-900 to-sky-600 text-white">
            <div class="flex justify-between h-full pl-32">
                <div class="self-end pb-32">
                    <h1 class="text-6xl font-semibold mb-6">Harness the power of</h1>
                    <h1 class="text-6xl font-semibold mb-6">a youth nation</h1>
                    <p class="mb-12">“Irrespective of any political party, Be a supporter of <br />good people who want to do something for the society.”</p>
                    <p class="mb-6">– Kapil Dev</p>
                    <nuxt-link to="/events">
                        <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-0">List your Events</a>
                    </nuxt-link>
                </div>
                <img class="self-end w-96 h-96" src="/guy2.png" alt="">
            </div>
        </div>
        <div class="h-screen w-96 bg-gradient-to-b from-sky-900 to-sky-600 text-white">
            <div class="flex justify-between h-full pl-32">
                <div class="self-end pb-32">
                    <h1 class="text-6xl font-semibold mb-6">Support Civic participation & drive</h1>
                    <h1 class="text-6xl font-semibold mb-6">impactful change</h1>
                    <p class="mb-12">“Action without thought is empty. Thought without action <br />is blind.”</p>
                    <p class="mb-6">– Kwame Nkrumah</p>
                    <nuxt-link to="/signup">
                        <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-0">Donate</a>
                    </nuxt-link>
                </div>
                <img class="self-end w-96 h-96" src="/guy3.png" alt="">
            </div>
        </div>
        </VueSlickCarousel>
    </div>
</template>
<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  name: "Slider",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        // dots: true,
        infinite: true,
        rows: 1,
        initialSlide: 0,
        speed: 500,
        slidesToShow: 1,
        slidesToScroll: 1,
        swipeToSlide: true,
        arrows: true,
      },
    }
  },
};
</script>