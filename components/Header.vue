<template>
    <nav class="flex items-center justify-between flex-wrap bg-teal px-12 py-6 bg-white">
  <div class="flex items-center flex-no-shrink text-white mr-6">
    <img src="/logo.png" alt="Logo" class="h-8 w-32 mr-2">
  </div>
  <div class="w-full block flex-col lg:flex lg:items-center lg:w-auto">
    <div class="text-sm lg:flex-grow">
    </div>
    <div>
        <input type="text" placeholder="Search" class="text-center outline-none border-solid border-2 py-2 border-sky-500 rounded placeholder:text-sky-500">
        <nuxt-link to="/">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Home</a>
        </nuxt-link>
        <nuxt-link to="/events">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Event</a>
        </nuxt-link>
        <nuxt-link to="/contact">
            <a class="inline-block text-sm w-28 text-center py-2 leading-none hover:border-transparent hover:text-teal hover:text-sky-500 hover:font-bold active:text-sky-500 active:font-bold mt-4 lg:mt-0">Contact Us</a>
        </nuxt-link>
        <nuxt-link to="/signin">
            <a class="inline-block text-sm w-28 text-center text-sky-500 py-2 leading-none border-solid border-2 border-sky-500 rounded hover:bg-gray-200 mt-4 lg:mt-0">Sign In</a>
        </nuxt-link>
        <nuxt-link to="/signup">
            <a class="inline-block text-sm w-28 text-center text-white py-2 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-0">Sign Up</a>
        </nuxt-link>
    </div>
  </div>
</nav>
</template>

<script>
export default {
    
}
</script>
