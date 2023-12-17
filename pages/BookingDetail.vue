<template>
  <div>
    <Header type='home'/>
    <div class="bg-violet-500 py-10">
      <div class="sm:mx-auto bg-white max-w-xl rounded-xl shadow-xl h-full mx-5">
        <div class="p-5">
          <div class="flex justify-between items-center mb-4">
            <div class="font-bold text-2xl">Payment</div>
            <svg class="h-6 w-6 text-violet-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 5v.01M12 12v.01M12 19v.01M12 6a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2z" />
            </svg>
          </div>
          <div class="block sm:flex border-2 border-gray-300 border-dashed rounded-lg mb-3">
            <div class="w-full sm:w-3/5 p-3 border-b-2 sm:border-r-2 border-dashed">
              <div class="lg:flex items-center">
                <img src="../assets/img/bidanjen.png" alt="bidan" class="lg:h-52 lg:w-52">
                <b class="text-xl">ANC</b>
              </div>
              <div class="grid grid-cols-2 mt-2 text-xs">
                <p class="text-gray-500">Name</p>
                <p class="text-gray-500">Method</p>
                <p class="mb-3">Tessa Salsabila</p>
                <p class="mb-3">Mandiri</p>
                <p class="text-gray-500">Terminal</p>
                <p class="text-gray-500">Total</p>
                <p class="mb-3">Kunjungan ANC ke-4</p>
                <p class="mb-3">Rp. 70.000,00</p>
              </div>
                <p class="text-xs text-gray-500">Date</p>
                <p class="text-xs">Monday, 18 December '23 - 12:33</p>
            </div>
              <img src="../assets/img/qr.png" alt="qr code" class="mx-auto my-auto">
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
