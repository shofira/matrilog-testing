<template>
  <div>
    <div class="flex justify-between my-5 font-bold">
      <div class="flex justify-between items-center">
        <h4 class="text-xl">Select Patient</h4>
        <p class="text-gray-700 text-sm">&nbsp; (3 patient found)</p>
      </div>
      <div class="flex justify-between items-center">
        <p class="text-sm mr-2">Sort by</p>
        <img src="../assets/img/sort.png" alt="sort" class="h-3 w-3">
      </div>
    </div>
    <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
      <div class="px-6 py-4">
        <b class="text-gray-700">Ny. Tessa Salsabila</b>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <b class="text-xl">ANC</b>
          <p class="text-gray-500 text-sm hidden md:flex justify-center"> Bidan Yurike</p>
          <div class="text-description text-center hidden sm:block">
            <b>Monday, 18 Dec '23'</b>
            <p>12:33</p>
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            Rp. 70.000,00
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
        </div>
      </div>
    </div>

    <div class="w-full bg-white rounded-lg shadow-lg mt-8 mt-3">
      <div class="px-6 py-4">
        <b class="text-gray-700">Ny. Moana Ranger</b>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <b class="text-xl">Contraseptive</b>
          <p class="text-gray-500 text-sm hidden md:flex justify-center"> Bidan Yurike</p>
          <div class="text-description text-center hidden sm:block">
            <b>Monday, 22 Dec '23'</b>
            <p>13:33</p>
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            Rp. 30.000,00
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
        </div>
      </div>
    </div>

    <div class="w-full bg-white rounded-lg shadow-lg mt-8 my-3">
      <div class="px-6 py-4">
        <b class="text-gray-700">Ny. Savira Frans</b>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 items-center space-x-5 my-3">
          <b class="text-xl">INC</b>
          <p class="text-gray-500 text-sm hidden md:flex justify-center"> Bidan Yasmine</p>
          <div class="text-description text-center hidden sm:block">
            <b>Monday, 18 Dec '23'</b>
            <p>12:33</p>
          </div>
          <p class="text-blue-500 text-sm hidden md:flex justify-center">
            Rp. 987.000,00
          </p>
          <button class="btn-auth-sm" @click="selectTicketing">Select</button>
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
