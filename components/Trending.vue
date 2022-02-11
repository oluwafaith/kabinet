<template>
<div>
<div class="grid gap-14 grid-cols-3 grid-rows-3 content-around ml-10 ">
<CardNew v-for="trend in trending" :key="trend.id" :trend="trend"/>
</div>
<div class="flex justify-center mt-14 mb-10">
<div class="flex  justify-center  text-white items-center text-md w-48 h-5 bg-sky-400 p-4 rounded-md"><nuxt-link to="/events">View All Events</nuxt-link></div>

</div>
</div>
</template>

<script>

import CardNew from "./CardNew.vue"
import trendData from "./trend.json"
export default {
name:'trending',
  components: { CardNew },
data(){
  return{
    trending: trendData
  }
}

}
</script>

