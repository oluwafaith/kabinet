<template>
  <div class="bg-white flex justify-center">
    <form
      class="rounded-lg pl-16 pr-16"
      :style="{ height: '1037px', white: '745px', background: '#FDFDFD' }"
    >
      <div class="">
        <header class="">
          <h2 class="font-bold text-2xl text-slate-500 text-center pb-16">Sign In</h2>
          <p class="text-sm text-slate-500 pb-8">
            Kindly enter your UserName/Email Address and Password to Sign In.

          </p>
          <p class="pb-8 text-center text-slate-500">
            Don't have an account?
            <nuxt-link to="/signup" class="text-teal-500">Sign Up</nuxt-link>
          </p>
        </header>

        <div class="">
          <div class="flex  w-96 bg-gray-200 rounded-lg mb-5" :style="{width:'470.75px'}">
            <span class="text-gray-400 pr-4 pl-2 pt-3 pb-3">
              <fa :icon="['fas', 'user']" />
            </span>
            <input
              class="w-96 placeholder:text-slate-400 bg-gray-200 outline-none"
              id="txt-input"
              type="text"
              placeholder="FirstName &amp; LastName "
              required
            />
          </div>



          <div class="flex w-96 bg-gray-200 items-center rounded-lg mb-5" :style="{width:'470.75px'}">
            <span class="text-gray-400 pr-4 pl-2 pt-3 pb-3">
              <fa :icon="['fas', 'lock']" />
            </span>
            <input
              class="w-96 placeholder:text-slate-400 bg-gray-200 outline-none"
              id="txt-input"
              type="password"
              placeholder="Password"
              required
            />
            <span class="text-slate-400">
              <fa :icon="['fas', 'eye']" />
            </span>
          </div>

  <div class="flex justify-between pb-4" >
    <div>
      <label class="" :style="{ position: 'relative',
  display: 'inline-block',
  width: '60px',
  height: '34px'}">
  <input type="checkbox" :style="{opacity: '0',
  width: '0',
  height: '0'}">
  <span class="slider round" :style="{   position: 'absolute',
  cursor: 'pointer',
  top: '0',
  left: '0',
  right: '0',
  bottom: '0',
  backgroundColor: '#ccc',
  webkitTransition: '.4s',
  transition: '.4s', borderRadius: '34px'}"></span>
</label>
      Remember Me</div>
    <div class="text-teal-500 ">Forgot Password?</div>
  </div>

          <button   class="flex items-center w-96 bg-gray-200 rounded-lg mb-5 pt-4 pb-4 j justify-center text-white " :style="{background: '#00ADEF', width:'470.75px'}">Submit</button >
        </div>

        <div class="flex justify-center mb-5 ">OR</div>
        <div class="flex items-center w-96 bg-gray-200 rounded-lg mb-5 pt-4 pb-4 justify-center text-white " :style="{background: '#5C67C8',width:'470.75px'} " >

        <span class="pr-6">  <fa :icon="['fab', 'facebook-f']"  /> </span>
          Connect with facebook
        </div>
        <div class="flex items-center w-96 bg-gray-200 rounded-lg mb-5 pt-4 pb-4 justify-center text-white" :style="{background: '#2E7CF6',width:'470.75px'} ">
        <span class="pr-6">  <fa :icon="['fab', 'google']" />
     </span>      Connect with Google
        </div>
        <div class="flex items-center w-96 bg-gray-200 rounded-lg mb-5 pt-4 pb-4 justify-center text-white" :style="{background: '#2E7CF6',width:'470.75px'} ">
        <span class="pr-6">  <fa :icon="['fab', 'twitter']" />
    </span>       Connect with Twitter
        </div>


      </div>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      email: "",
      password: "",
      error: null,
    };
  },
};
</script>
