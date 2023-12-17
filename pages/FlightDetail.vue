<template>
  <div>
    <Header type='home'/>
      <div class="bg-gray-200 pb-5">
        <div class="bg-violet-500 rounded-b-3xl">
          <h1 class="text-violet-500 text-8xl">asdf</h1>
        </div>
        <div class="container block md:flex justify-between py-10 gap-10">
          <div class="w-full">
            <h4 class="text-xl font-bold mb-5">Patient Personal Info</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <p class="text-description-sm">Full Name</p>
                <input class="input-form" type="text" placeholder="Mike Kowalski">
                <div class="flex">
                  <div>
                    <p class="text-description-sm">NIK</p>
                    <input class="input-form" type="number" placeholder="78237595">
                  </div>
                  <div>
                    <p class="text-description-sm">BPJS Number</p>
                    <input class="input-form" type="number" placeholder="G2P1A0">
                  </div>
                  <div>
                    <p class="text-description-sm">Phone Number</p>
                    <input class="input-form" type="number" placeholder="+62 27186558">
                  </div>
                </div>
                <div class="flex">
                  <div>
                    <p class="text-description-sm">GPA</p>
                    <input class="input-form" type="Text" placeholder="78237595">
                  </div>
                  <div>
                    <p class="text-description-sm">Gestational Age</p>
                    <input class="input-form" type="number" placeholder="38 week">
                  </div>
                  <div>
                    <p class="text-description-sm">Estimated Date of birth</p>
                    <input class="input-form" type="date" placeholder="02/03/2023">
                  </div>
                </div>

                <div class="flex items-center bg-red-200 text-red-700 text-sm px-4 py-3 rounded-lg my-3" role="alert">
                  <svg class="h-5 w-5 mr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z" />
                  </svg>
                  <p>Make sure the customer data is correct.</p>
                </div>
              </div>
            </div>

            <h4 class="text-xl font-bold my-5">Payment Details</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <div class="flex justify-between my-3 items-center">
                  <b> $ Total </b>
                  <p class="text-blue-500 text-sm">Rp. 70.000,00</p>
                </div>
                <hr>
              </div>
            </div>
            <button class="btn-auth mt-10 mb-5" @click="payment">Proceed to Payment</button>
          </div>

          <div class="w-full">
            <h4 class="text-xl font-bold mb-5">Physical Checkup</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <p class="text-description-sm">Complaints of pain</p>
                <input class="input-form" type="textarea" placeholder="Mual">
                <p class="text-description-sm">Kunjungan ANC Ke-</p>
                <select class="input-form">
                  <option>ANC 1</option>
                  <option>ANC 2</option>
                  <option>ANC 3</option>
                </select>
                <div class="flex">
                  <div>
                    <p class="text-description-sm">TB</p>
                    <input class="input-form" type="number" placeholder="165 cm">
                  </div>
                  <div>
                    <p class="text-description-sm">BB</p>
                    <input class="input-form" type="number" placeholder="45 Kg">
                  </div>
                  <div>
                    <p class="text-description-sm">TD</p>
                    <input class="input-form" type="text" placeholder="120/80">
                  </div>
                  <div>
                    <p class="text-description-sm">N</p>
                    <input class="input-form" type="number" placeholder="80x/menit">
                  </div>
                  <div>
                    <p class="text-description-sm">S</p>
                    <input class="input-form" type="number" placeholder="37.5 ℃">
                  </div>
                </div>
                <p class="text-description-sm">Terapi Obat</p>
                <input class="input-form" type="text" placeholder="Fe 1x1, Asam Folat">
              </div>
            </div>
          </div>

        </div>
      </div>
    <Footer />
  </div>
</template>

<script>
export default {
  methods: {
    payment() {
      this.$router.push('/bookingdetail')
    }
  }
}
</script>
