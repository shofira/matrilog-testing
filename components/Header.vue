<template>
  <div>
    <nav class="container block lg:flex justify-between gap-4 py-5 lg:py-2">
      <div class="flex justify-between">
        <nuxt-link to="/" class="flex lg:items-center">
          <img src="../assets/img/logomatrilog.png" class="w-10 h-10 mt-1" alt="logo matrilog">
          <b class="text-xl text-gray-800 tracking-wider">Matrilog</b>
        </nuxt-link>
        <div class="flex lg:hidden cursor-pointer" @click="collapse">
          <svg class="h-4 w-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </div>
      </div>
      <div class="container flex flex-col lg:flex-row lg:items-center lg:flex justify-between text-sm py-3 hidden" id="collapse-nav">
        <div class="flex flex-col lg:flex-row lg:items-center">
          <button class="search-box">
            <Icons type='search' class="ml-3"/>
            <input type="text" class="w-full bg-transparent text-gray-600 text-sm px-3 py-3 focus:outline-none rounded-md" placeholder="Where you want to go?">
          </button>
        </div>
        <div class="flex flex-col lg:flex-row lg:items-center lg:space-x-8 font-bold mb-3">
          <nuxt-link to="/flight" class="block py-2">Find Patient</nuxt-link>
          <nuxt-link to="/mybooking" class="block py-2">BPJS</nuxt-link>
          <nuxt-link to="/mybooking" class="block py-2">Schedule</nuxt-link>
          <nuxt-link to="/mybooking" class="block py-2">Our Teams</nuxt-link>
        </div>

        <!-- Condition -->
        <div class="flex flex-col lg:flex-row lg:items-center">
          <div v-if="type==='home'" class="flex space-x-8 items-center">
            <img src="../assets/img/message.png" alt="message" class="h-4 w-4">
            <img src="../assets/img/bell.png" alt="notification" class="h-5 w-4">
            <nuxt-link to="/profile">
              <img src="../assets/img/profile.png" alt="profile" class="block py-2 px-4 w-4/5 img-profile">
            </nuxt-link>
          </div>
          <div v-else>
            <nuxt-link to="/splashscreen" class="btn-auth-sm">
              Sign Up
            </nuxt-link>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  props: ['type'],
  methods: {
    collapse() {
      const overlay = document.querySelector('#collapse-nav')
      if (overlay.classList.contains('flex')) {
        overlay.classList.remove('flex')
        overlay.classList.add('hidden')
      } else {
        overlay.classList.remove('hidden')
        overlay.classList.add('flex')
      }
    }
  }
}
</script>
