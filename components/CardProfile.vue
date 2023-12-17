<template>
  <div>
    <div class="w-full bg-white rounded-lg shadow-lg">
      <div class="p-6">
          <img src="../assets/img/bigProfile.png" alt="profile" class=" mx-auto">
        <div class="text-center">
          <button class="btn-outline-auth-sm my-4">
            <input type="file" class="hidden">
            Select Photo
          </button>
          <h3 class="text-lg font-bold">Mike Kowalski</h3>
          <p class="text-description">Medan, Indonesia</p>
        </div>
        <div class="container flex justify-between text-sm">
          <p class="font-bold">Cards</p>
          <p class="text-blue-600">+ Add</p>
        </div>
        <div class="container bg-blue-500 text-white mx-auto my-3 px-5 py-3 rounded-lg shadow">
          <b class="tracking-widest">4441 1235 5512 5551</b>
          <div class="flex justify-between text-sm leading-8">
            <p class="text-gray-400">Xcards</p>
            <p class="text-gray-400">$ 1,440.2</p>
          </div>
        </div>
        <div class="container mx-5 text-sm font-bold leading-10">
          <nuxt-link to="/profile" class="flex items-center text-blue-600">
            <Icons type='user'/> Profile
          </nuxt-link>
          <nuxt-link to="/mybooking" class="flex items-center">
            <Icons type='star'/> My Review
          </nuxt-link>
          <nuxt-link to="" class="flex items-center">
            <Icons type='setting'/> Setting
          </nuxt-link>
          <nuxt-link to="/" class="flex text-red-600 items-center">
            <Icons type='logout'/> Logout
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>