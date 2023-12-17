<template>
  <div>
    <Header type='home'/>
    <div class="bg-gray-200 pb-10">
      <div class="bg-blue-500 rounded-b-3xl flex items-center">
        <img src="../assets/img/plane.png" alt="plane background" class="w-2/6 sm:w-1/6">
        <div class="container leading-8 hidden md:block">
          <div class="flex space-x-24 text-gray-300 text-xs">
            <p>From</p>
            <p>To</p>
          </div>
          <div class="flex items-center space-x-6 text-gray-300 text-xs">
            <!-- <img src="../assets/img/whiteheadeplane.png" alt=""> -->
            <b>Medan (IDN)</b>
            <img src="../assets/img/whiteswitch.png" alt="to" class="h-3 w-3">
            <b>Tokyo (JPN)</b>
          </div>
          <p class="text-gray-300 text-sm">Monday, 20 July 20 • 6 Passenger • Economy</p>
        </div>
        <b class="text-gray-100 text-xs hidden md:block">Change Search</b>
      </div>
      <div class="container block md:flex gap-10">
        <div class="w-1/2">
          <FilterBox />
        </div>
        <div class="w-full">
          <CardFlight />
        </div>
      </div>
    </div>
    <Footer/>
  </div>
</template>