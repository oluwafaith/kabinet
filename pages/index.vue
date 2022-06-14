<template>
  <div>
    <ImageSlider />
    <!-- <div id="app">
      <NewSlider />
    </div> -->
    <div class="px-32 py-6 bg-sky-900 text-white">
      <h4>Latest Events!</h4>
    </div>
    <EventsSlider />
    <div class="px-32 py-6 bg-sky-900 text-white">
      <h4>Trending Events</h4>
    </div>
    <div class="mt-20">
    <Trending/>
    </div>
  </div>
</template>

<script>
import Trending from '../components/Trending.vue'
export default {
  components: { Trending },
  name: 'IndexPage',
}
</script>

<style>
</style>
