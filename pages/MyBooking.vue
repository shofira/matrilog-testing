<template>
  <div>
    <Header type='home'/>
    <div class="bg-gray-200 py-10">
      <div class="container block md:flex gap-10">
        <CardProfile />
        <div class="block">
          <div class="w-full bg-white rounded-lg shadow-lg mt-10 md:mt-0">
            <div class="px-6 py-4">
              <b class="text-tracking">My Booking</b>
              <div class="flex justify-between items-center">
                <p class="font-bold text-2xl">My Booking</p>
                <p class="text-blue-600">Order History</p>
              </div>
              <p class="text-transparent text-base hidden sm:flex">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem 
              </p>
            </div>
          </div>

          <div class="col-span-3 bg-white rounded-lg shadow-lg mt-5">
            <div class="px-6 py-4">
              <b class="text-xs tracking-widest uppercase mb-2">
                Monday, 20 July '20 - 12:33
              </b>
              <div class="flex items-center space-x-3 my-3">
                <b class="text-xl">IDN</b>
                <img src="../assets/img/greysmallplane.png" alt="">
                <b class="text-xl">JPN</b>
              </div>
              <p class="text-description">Garuda Indonesia, AB-221</p>
              <hr class="my-3">
              <div class="flex justify-between items-center gap-4 text-sm">
                <b class="text-gray-700">Status</b>
                <button class="btn-waiting">Waiting  for payment</button>
                <nuxt-link to="/bookingdetail" class="font-bold text-blue-600 hidden sm:flex">
                  View Details
                  <Icons type='button-bottom' />
                </nuxt-link>
              </div>
            </div>
          </div>
          
          <div class="col-span-3 bg-white rounded-lg shadow-lg mt-5">
            <div class="px-6 py-4">
              <b class="text-xs tracking-widest uppercase mb-2">
                Monday, 20 July '20 - 12:33
              </b>
              <div class="flex items-center space-x-3 my-3">
                <b class="text-xl">IDN</b>
                <img src="../assets/img/greysmallplane.png" alt="">
                <b class="text-xl">JPN</b>
              </div>
              <p class="text-description">Garuda Indonesia, AB-221</p>
              <hr class="my-3">
              <div class="flex justify-between items-center gap-4 text-sm">
                <b class="text-gray-700">Status</b>
                <button class="btn-done">Eticket issued</button>
                <nuxt-link to="/bookingdetail" class="font-bold text-blue-600 hidden sm:flex">
                  View Details
                  <Icons type='button-bottom' />
                </nuxt-link>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>