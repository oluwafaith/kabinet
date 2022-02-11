<template>
<div>
  <h1 class="text-3xl font-bold underline">
    Home Page
  </h1>
  <Trending/>
</div>
</template>

<script>
import Trending from '../components/Trending.vue'
export default {
  components: { Trending },
  name: 'IndexPage',

}
</script>
