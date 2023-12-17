<template>
  <div class="flex items-center text-center justify-center">
    <div class="max-w-md">
      <div class="p-3">
        <img src="../assets/img/logomatrilog.png" class="m-auto md:max-w-xs" />
        <h1 class="text-3xl mb-2 font-bold"> Get Started </h1>
        <p class="text-sm text-gray-600">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates sequi commodi voluptate quos explicabo labore vel!
        </p>
      </div>
      <div class="my-4">
        <nuxt-link to="/register" class="btn-auth mr-4 sm:mr-0 sm:block mb-5" >
          Create My Account
        </nuxt-link>
        <nuxt-link to="/login" class="btn-outline-auth sm:block" >
          Sign In
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
