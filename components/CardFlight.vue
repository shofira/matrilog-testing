<template>
  <div>
    <div class="flex justify-between my-5 font-bold">
      <div class="flex justify-between items-center">
        <h4 class="text-xl">Select Ticket</h4>
        <p class="text-gray-700 text-sm">&nbsp; (6 flight found)</p>
      </div>
      <div class="flex justify-between items-center">
        <p class="text-sm mr-2">Sort by</p>
        <img src="../assets/img/sort.png" alt="sort" class="h-3 w-3">
      </div>
    </div>
    <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
      <div class="px-6 py-4">
        <div class="flex items-center space-x-5 mb-6">
          <img src="../assets/img/garuda.png" alt="airline">
          <b class="text-gray-700">Garuda Indonesia</b>
        </div>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <div class="flex space-x-5 items-center">
            <div>
              <b class="text-xl">IDN</b>
              <p class="text-description text-xs">12:33</p>
            </div>
            <img src="../assets/img/greysmallplane.png" alt="plane to">
            <div>
              <b class="text-xl">JPN</b>
              <p class="text-description text-xs">15:21</p>
            </div>
          </div>

          <div class="text-description text-center hidden sm:block">
            <b>3 hours 11 minutes</b>
            <p>(1 transit)</p>
          </div>
          <div class="hidden md:flex space-x-5 justify-center">
            <img src="../assets/img/bag.png" alt="luggage">
            <img src="../assets/img/food.png" alt="meal">
            <img src="../assets/img/wifi.png" alt="wifi">
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            $ 2,00/pax
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
        </div>
        <div class="flex items-center space-x-5 text-sm my-3">
          <nuxt-link to="/bookingdetail" class="font-bold text-blue-600 flex">
            View Details
            <Icons type='button-bottom' />
          </nuxt-link>
        </div>
      </div>
    </div>

    <div class="w-full bg-white rounded-lg shadow-lg mt-8">
      <div class="px-6 py-4">
        <div class="flex items-center space-x-5 mb-6">
          <img src="../assets/img/lion_air.png" alt="airline">
          <b class="text-gray-700">Lion Air</b>
        </div>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <div class="flex space-x-5 items-center">
            <div>
              <b class="text-xl">IDN</b>
              <p class="text-description text-xs">12:33</p>
            </div>
            <img src="../assets/img/greysmallplane.png" alt="plane to">
            <div>
              <b class="text-xl">JPN</b>
              <p class="text-description text-xs">15:21</p>
            </div>
          </div>

          <div class="text-description text-center hidden sm:block">
            <b>3 hours 11 minutes</b>
            <p>(1 transit)</p>
          </div>
          <div class="hidden md:flex space-x-5 justify-center">
            <img src="../assets/img/bag.png" alt="luggage">
            <img src="../assets/img/food.png" alt="meal">
            <img src="../assets/img/wifi.png" alt="wifi">
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            $ 2,00/pax
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
        </div>
        <div class="flex items-center space-x-5 text-sm my-3">
          <nuxt-link to="/bookingdetail" class="font-bold text-blue-600 flex">
            View Details
            <Icons type='button-bottom' />
          </nuxt-link>
        </div>
      </div>
    </div>

    <div class="w-full bg-white rounded-lg shadow-lg mt-8">
      <div class="px-6 py-4">
        <div class="flex items-center space-x-5 mb-6">
          <img src="../assets/img/air_asia.png" alt="airline">
          <b class="text-gray-700">Air Asia</b>
        </div>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <div class="flex space-x-5 items-center">
            <div>
              <b class="text-xl">IDN</b>
              <p class="text-description text-xs">12:33</p>
            </div>
            <img src="../assets/img/greysmallplane.png" alt="plane to">
            <div>
              <b class="text-xl">JPN</b>
              <p class="text-description text-xs">15:21</p>
            </div>
          </div>

          <div class="text-description text-center hidden sm:block">
            <b>3 hours 11 minutes</b>
            <p>(1 transit)</p>
          </div>
          <div class="hidden md:flex space-x-5 justify-center">
            <img src="../assets/img/bag.png" alt="luggage">
            <img src="../assets/img/food.png" alt="meal">
            <img src="../assets/img/wifi.png" alt="wifi">
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            $ 2,00/pax
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
        </div>
        <div class="flex items-center space-x-5 text-sm my-3">
          <nuxt-link to="/bookingdetail" class="font-bold text-blue-600 flex">
            View Details
            <Icons type='button-bottom' />
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    selectTicketing() {
      this.$router.push('/flightdetail')
    }
  }
}
</script>