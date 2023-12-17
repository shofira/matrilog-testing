<template>
  <div>
    <Header type='home'/>
    <div class="bg-blue-500 py-10">
      <div class="sm:mx-auto bg-white max-w-xl rounded shadow-xl h-full mx-5">
        <div class="p-5">
          <div class="flex justify-between items-center mb-6">
            <div class="font-bold text-2xl">Booking Pass</div>
            <svg class="h-6 w-6 text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 5v.01M12 12v.01M12 19v.01M12 6a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2z" />
            </svg>
          </div>
          <div class="block sm:flex border-2 border-gray-300 border-dashed rounded-lg mb-3">
            <div class="w-full sm:w-3/5 p-4 border-b-2 sm:border-r-2 border-dashed">
              <div class="flex items-center space-x-3">
                <img src="../assets/img/garuda.png" alt="airline">
                <b class="text-xl">IDN</b>
                <img src="../assets/img/greysmallplane.png" alt="">
                <b class="text-xl">JPN</b>
              </div>
              <div class="grid grid-cols-2 text-xs my-4">
                <p class="text-gray-500">Code</p>
                <p class="text-gray-500">Class</p>
                <p class="mb-3">AB-221</p>
                <p class="mb-3">Economy</p>
                <p class="text-gray-500">Terminal</p>
                <p class="text-gray-500">Gate</p>
                <p class="mb-3">AB-221</p>
                <p class="mb-3">Economy</p>
              </div>
                <p class="text-xs text-gray-500">Departure</p>
                <p class="text-xs">Monday, 20 July '20 - 12:33</p>
            </div>
              <img src="../assets/img/qr.png" alt="qr code" class="mx-auto my-auto">
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>