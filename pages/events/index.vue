<template>
<div>
<CardNew/>
<!-- <card-new/> -->
<div class="flex justify-center mt-14 mb-10">
<div class="flex  justify-center  text-white items-center mt-10 mb-10 text-md w-48 h-5 bg-sky-400 p-4 rounded-md"><nuxt-link to="/events">Load More</nuxt-link></div>
</div>
</div>
</template>

<script>
import CardNew from "../../components/Card.vue"
export default {

  components: { CardNew },


}
</script>

