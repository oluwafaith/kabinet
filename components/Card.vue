<template>
  <div class="grid gap-14 grid-cols-3 grid-rows-3 content-around ml-10 ">
  <!-- <div class="flex flex-wrap flex-row justify-around mb-10"> -->
    <div v-for="trend in trending" :key="trend.id" class="w-96 rounded-lg shadow-md ">
      <!-- img -->
      <div class="h-56 w-96">
        <img :src="trend.img" alt="img" class="object-none h-full w-full rounded-t-lg " />
      </div>

      <!-- details -->
      <div class="h-64 rounded-t-2xl rounded-b-lg shadow-lg  p-5 text-slate-600 ">
        <div class="text-xl font-bold pb-5">{{ trend.name }}</div>

        <div class="flex justify-between text-sm pb-4">
          <span>
            <fa :icon="['fas', 'clock']" />
           <span class="text-slate-600"> {{ trend.date }} </span>
            </span
          >
          <span>
            <fa :icon="['fas', 'calendar-days']" />
            {{ trend.time }}</span
          >
        </div>

        <div class="flex justify-between text-sm ">
          <span>
            <fa :icon="['fas', 'location-dot']" />
            {{ trend.location }}
            </span
          >

          <div class="flex justify-center text-white items-center  mb-3 h-10 w-36 text-xl  bg-sky-400 pt-6 pb-6  rounded-md"> <nuxt-link to="/events/:id">Read More  </nuxt-link></div>
        </div>

        <div class="pt-2 pb-3">
          <div class="w-80 h-0.5 bg-slate-200 "></div>
          </div>

        <div class="flex justify-between text-lg">
          <span>
            <fa :icon="['fas', 'thumbs-up']" />
            interested</span
          >
          <span>
            <fa :icon="['fas', 'share-nodes']" />
            share</span
          >
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      trending: [
        {
          id: 1,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_NkkTJ6MiRWI.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 2,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 3,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 4,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 5,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 6,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 7,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 8,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
        {
          id: 9,
          name: " Civic engagement through votes; importance and processes involved.",
          img: "/trend/unsplash_9kbaq1xoIr0.png",
          date: "Friday, Dec. 2, 2021.",
          time: "8:00pm  - 12:00am WAT",
          location: "Golden Tulip Hotel, Marina, Lagos. ",
        },
      ],
    };
  },
};
</script>
