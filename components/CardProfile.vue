<template>
  <div>
    <div class="w-full bg-white rounded-lg shadow-lg">
      <div class="p-6">
          <img src="../assets/img/person1.jpg" alt="profile" class="h-24 w-18 rounded-full mx-auto">
        <div class="text-center">
          <button class="btn-outline-auth-sm my-4">
            <input type="file" class="hidden">
            Select Photo
          </button>
          <h3 class="text-lg font-bold">Jasmine Kowalski</h3>
          <p class="text-description">2th working</p>
        </div>
        <div class="container bg-violet-500 text-white mx-auto my-3 px-4 py-3 rounded-lg shadow">
          <b class="tracking-widest">4441 1235 5512 5551</b>
          <div class="flex justify-between text-sm leading-8">
            <p class="text-white-400">STR</p>
            <p class="lg:text-xs lg:mt-2 text-white-400">Valid till 2/5/25</p>
          </div>
        </div>
        <div class="container mx-5 text-sm font-bold leading-10">
          <nuxt-link to="/profile" class="flex items-center text-violet-600">
            <Icons type='user'/> Profile
          </nuxt-link>
          <nuxt-link to="" class="flex items-center">
            <Icons type='star'/> My Schedule
          </nuxt-link>
          <nuxt-link to="" class="flex items-center">
            <Icons type='setting'/> Setting
          </nuxt-link>
          <nuxt-link to="/login" class="flex text-red-600 items-center">
            <Icons type='logout'/> Logout
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>
