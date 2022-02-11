<template>
    <div>
        <VueSlickCarousel v-bind="settings">
        <div class="bg-sky-900 text-white text-center border-t-2 border-b-2 border-white pt-12 pb-12">
            <div class="pl-32 pr-32">
                <h1 class="text-3xl font-semibold">Civic engagement through votes;</h1>
                <h1 class="text-3xl font-semibold mb-6">importance and processes involved.</h1>
                <div class="flex justify-around">
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="calendar"/>
                        <div>Friday, Dec. 2, 2021.</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="clock"/>
                        <div>8:00pm - 12:00am WAT</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="location"/>
                        <div>Golden Tulip Hotel, Marina, Lagos.</div>
                    </div>
                </div>
                <nuxt-link to="/more">
                    <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-12">Read More</a>
                </nuxt-link>
            </div>
        </div>
        <div class="bg-sky-900 text-white text-center border-t-2 border-b-2 border-white pt-12 pb-12">
            <div class="pl-32 pr-32">
                <h1 class="text-3xl font-semibold">Civic engagement through votes;</h1>
                <h1 class="text-3xl font-semibold mb-6">importance and processes involved.</h1>
                <div class="flex justify-around">
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="calendar"/>
                        <div>Friday, Dec. 2, 2021.</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="clock"/>
                        <div>8:00pm - 12:00am WAT</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="location"/>
                        <div>Golden Tulip Hotel, Marina, Lagos.</div>
                    </div>
                </div>
                <nuxt-link to="/more">
                    <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-12">Read More</a>
                </nuxt-link>
            </div>
        </div>
        <div class="bg-sky-900 text-white text-center border-t-2 border-b-2 border-white pt-12 pb-12">
            <div class="pl-32 pr-32">
                <h1 class="text-3xl font-semibold">Civic engagement through votes;</h1>
                <h1 class="text-3xl font-semibold mb-6">importance and processes involved.</h1>
                <div class="flex justify-around">
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="calendar"/>
                        <div>Friday, Dec. 2, 2021.</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="clock"/>
                        <div>8:00pm - 12:00am WAT</div>
                    </div>
                    <div class="flex justify-center items-center">
                        <fa class="mr-2" icon="location"/>
                        <div>Golden Tulip Hotel, Marina, Lagos.</div>
                    </div>
                </div>
                <nuxt-link to="/more">
                    <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-12">Read More</a>
                </nuxt-link>
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