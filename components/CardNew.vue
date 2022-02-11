<template>


    <div  class="w-96  rounded-lg shadow-md bg-cover bg-center p-0 m-0 "   :style="{
          backgroundImage: `url(${trend.img})`,
           backgroundSize: 'cover',
          backgroundRepeat: 'no-repeat',
         

        }">
      <!-- img -->
      <div class="h-56 w-96" :id="trend.id">
        <img :src="trend.img" alt="img" class="object-none h-full w-full rounded-t-lg " />
      </div>

      <!-- details -->
      <div class="h-64 rounded-t-2xl rounded-t-2xl rounded-b-lg shadow-t-lg  shadow-lg  bg-white p-5 text-slate-600 ">
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

          <div class="flex justify-center text-white items-center  mb-3 h-10 w-36 text-xl  bg-sky-400 pt-6 pb-6  rounded-md"> <nuxt-link :to="{ name: 'events-id', params: { id: trend.id } }">Read More  </nuxt-link></div>



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

</template>

<script>
export default {
   name: 'trend',
   props:['trend']
  };
</script>

