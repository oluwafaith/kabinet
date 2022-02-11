<template>

    <nav :style="{
    bottom:0, }" class="flex items-center   mb-10 justify-between flex-wrap bg-teal px-12 py-6 bg-white">
      <div class="w-full h-0.5 bg-slate-200"></div>
  <div class="flex items-center mt-10 flex-no-shrink text-white mr-6">
    <img src="/logo.png" alt="Logo" class="h-8 w-32 mr-2">
  </div>
  <div class="w-full block flex-col lg:flex lg:items-center lg:w-auto">
    <div class="text-sm lg:flex-grow">
    </div>
    <div>
        <nuxt-link to="/">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Home</a>
        </nuxt-link>
        <nuxt-link to="/events">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Event</a>
        </nuxt-link>
        <nuxt-link to="/contact">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Contact Us</a>
        </nuxt-link>

    </div>
  </div>
</nav>
</template>

<script>
export default {

}
</script>
