<template>
  <div>
    <Header type='home'/>
    <div class="bg-gray-200 py-10">
      <div class="container block md:flex gap-10">
        <CardInfo />
        <div class="block">
          <div class="w-full bg-white rounded-lg shadow-lg mt-10 md:mt-0">
            <div class="px-6 py-3">
              <b class="text-tracking">Medical Records</b>
              <div class="flex justify-between items-center my-2">
                <p class="font-bold text-2xl">Ny. Tessa Salsabila</p>
                <p class="text-violet-600 text-sm">Load More History</p>
              </div>
              <p class="text-transparent text-base hidden sm:flex">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem
              </p>
            </div>
          </div>
          <!-- payment waiting -->
          <div class="col-span-3 bg-white rounded-lg shadow-lg mt-5">
            <div class="px-6 py-4">
              <b class="text-xs tracking-widest uppercase">
                Monday, 20 July '20 - 12:33
              </b>
              <h1 class="text-xl my-2"><b>ANC</b></h1>
              <p class="text-description">Kunjungan ANC 4 - Asam Folat, Fe 1x1</p>
              <hr class="my-3">
              <div class="flex justify-between items-center gap-4 text-sm">
                <b class="text-gray-700">Status</b>
                <nuxt-link to="/bookingdetail">
                  <button class="btn-waiting">Waiting  for payment</button>
                </nuxt-link>
                <nuxt-link to="/flightdetail" class="font-bold text-blue-600 hidden sm:flex">
                  View Details
                  <Icons type='button-bottom' />
                </nuxt-link>
              </div>
            </div>
          </div>
          <!-- payment done -->
          <div class="col-span-3 bg-white rounded-lg shadow-lg mt-5">
            <div class="px-6 py-4">
              <b class="text-xs tracking-widest uppercase">
                Monday, 20 July '20 - 12:33
              </b>
              <h1 class="text-xl my-2"><b>ANC</b></h1>
              <p class="text-description">Kunjungan ANC 3 - Asam Folat, Fe 1x1</p>
              <hr class="my-3">
              <div class="flex justify-between items-center gap-4 text-sm">
                <b class="text-gray-700">Status</b>
                <nuxt-link to="">
                  <button class="btn-done">Paid Off</button>
                </nuxt-link>
                <nuxt-link to="/flightdetail" class="font-bold text-blue-600 hidden sm:flex">
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
