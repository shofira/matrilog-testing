<template>
  <div>
    <Header type='home'/>
      <div class="bg-gray-200 pb-5">
        <div class="bg-blue-500 rounded-b-3xl">
          <img src="../assets/img/plane.png" alt="plane background" class="w-2/6 sm:w-1/6">
        </div>
        <div class="container block md:flex justify-between py-10 gap-10">
          <div class="w-full">
            <h4 class="text-xl font-bold mb-5">Contact Person Details</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <p class="text-description-sm">Full Name</p>
                <input class="input-form" type="text" placeholder="Mike Kowalski">
                <p class="text-description-sm">Email</p>
                <input class="input-form" type="email" placeholder="mikeFlight@ankasa.com">
                <p class="text-description-sm">Phone Number</p>
                <input class="input-form" type="number" placeholder="+62 78237595">
                <div class="flex items-center bg-red-200 text-red-700 text-sm px-4 py-3 rounded-lg my-3" role="alert">
                  <svg class="h-5 w-5 mr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z" />
                  </svg>
                  <p>Make sure the customer data is correct.</p>
                </div>
              </div>
            </div>

            <h4 class="text-xl font-bold my-5">Passenger Details</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <p class="text-description-sm">Title</p>
                <select class="input-form">
                  <option>Mr.</option>
                  <option>Mrs.</option>
                </select>
                <p class="text-description-sm">Full Name</p>
                <input class="input-form" type="text" placeholder="Mike Kowalski">
                <p class="text-description-sm">Nasionality</p>
                <select class="input-form">
                  <option selected disabled>Indonesia</option>
                </select>
              </div>
            </div>

            <h4 class="text-xl font-bold my-5">Passenger Details</h4>
            <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4">
                <div class="flex justify-between my-3 items-center">
                  <b>
                    <input class="mr-2 leading-tight" type="checkbox">
                    Travel Insurance
                  </b>
                  <p class="text-blue-500 text-sm">$ 2,00/pax</p>
                </div>
                <hr>
                <p class="text-gray-700 text-sm my-3">
                  Get travel compensation up to $ 10.000,00
                </p>
              </div>
            </div>
            <button class="btn-auth mt-10 mb-5" @click="payment">Proceed to Payment</button>
          </div>

          <div class="w-full">
            <h4 class="text-xl font-bold mb-5">Flight Details</h4>
            <div class="w-full bg-white rounded-xl shadow-lg mt-8 md:mt-0">
              <div class="px-6 py-4 leading-10">
                <div class="flex items-center space-x-5">
                  <img src="../assets/img/garuda.png" alt="airline">
                  <b class="text-gray-700">Garuda Indonesia</b>
                </div>
                <div class="flex items-center space-x-5 my-3">
                  <b class="text-xl">Medan (IDN)</b>
                  <img src="../assets/img/greysmallplane.png" alt="plane to">
                  <b class="text-xl">Tokyo (JPN)</b>
                </div>
                <p class="text-gray-700 text-sm">Sunday, 15 August 2020 • 12:33 - 15:21</p>
                <hr>
                <div class="flex justify-between my-3 items-center">
                  <b>Total Payment</b>
                  <p class="text-blue-500 text-sm flex items-center">$ 145,00
                    <Icons type='button-bottom' />
                  </p>
                </div>
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
      this.$router.push('/mybooking')
    }
  }
}
</script>