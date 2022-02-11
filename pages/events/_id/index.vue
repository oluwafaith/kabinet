<template>
  <div>
    <div v-for="trend in Trends" :trend="trend" :key="trend.id">
      <div
        class="w-full "
        :style="{
          backgroundImage: `url(${trend.img})`,
          backgroundSize: 'contain',
          backgroundRepeat: 'no-repeat',
          height: '486px',

        }"
      >
        <nuxt-link :to="{ name: 'events' }">Back </nuxt-link>
      </div>

      <div class="flex items-center bg-blue-900 h-20 text-white">
        <div class="flex text-lg pl-20">
          <span class="pr-20">
            <fa :icon="['fas', 'thumbs-up']" />
            interested</span
          >
          <span>
            <fa :icon="['fas', 'share-nodes']" />
            share</span
          >
        </div>
      </div>

      <div
        class="flex justify-between flex-row pl-16 pr-16"
        :style="{ height: '700px' }"
      >
        <!-- left -->
        <div class="w-7/12" :style="{ width: '700px' }">
          <div class="text-xl mt-4 font-bold pb-5 text-slate-600" :style="{ fontSize: '32px' }">
            {{ trend.name }}
          </div>
          <div class="break-all align-middle text-justify text-xl text-slate-500">
            {{ trend.details }}
          </div>
          <p class="font-bold text-xl pb-2 pt-2 text-slate-600 ">Highlights</p>
          <ul class="text-lg text-slate-500 list-disc">
            <li>
              Sparking dialogue, igniting inspiration, and diving deep into the
              current issues facing the fashion.
            </li>
            <li>
              An opportunity for the global fashion community to explore
              observations and experiences.
            </li>
            <li>
              Strategise actionable and innovative ideas for businesses and
              brands.
            </li>
          </ul>
        </div>
        <!-- right -->
        <div class="w-4/12" :style="{ width: '425px' }">
          <div
            class="flex justify-center pt-4 pb-4 mt-4 mb-6 bg-sky-500 text-2xl text-white"
            :style="{ width: '425px' }"
          >
            Details
          </div>
          <div>
            <!-- <div class="h-96 w-1 bg-slate-300">
            </div> -->
            <p class="mb-2 text-slate-600 font-bold">Date:</p>
          <span class="text-slate-600 ">{{ trend.date }}</span>
          <p class="mt-2 mb-2 text-slate-600 font-bold">Time:</p>
          <span class="text-slate-600 ">{{ trend.time }}</span>
          <p class="mt-2 mb-2 text-slate-600 font-bold">Location:</p>
          <span class="text-slate-600 ">{{ trend.location }}</span>
          <p class="mt-2 mb-2 text-slate-600 font-bold">Entry Fee:</p>
          <span class="text-slate-600 ">{{trend.fee}}</span>
          <p class="mt-2 mb-2 text-slate-600 font-bold">Official Link:</p>
          <span class="text-slate-600 "> {{trend.link}}</span>
            </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
import trendData from "../../../components/trend.json";
export default {
  data() {
    return {
      trending: trendData,
    };
  },
  computed: {
    Trends() {
      return this.trending.filter((trend) => trend.id == this.$route.params.id);
    },
  },
};
</script>
