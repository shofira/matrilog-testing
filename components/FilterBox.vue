<template>
  <div>
    <div class="hidden md:block">
      <div class="flex justify-between my-5">
        <h4 class="text-xl font-bold">Filter</h4>
        <p class="text-sm text-violet-600">reset</p>
      </div>
      <div class="w-full bg-white rounded-lg shadow-lg mt-8 md:mt-0">
        <div class="px-6 py-4">
          <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Services</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>ANC</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>INC</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>PNC & BBL</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Contraseptive</p>
            <input class="mr-4" type="checkbox">
          </div>
          <hr>
          <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Midwife</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Jennifer</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Yasmin</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Yurike</p>
            <input class="mr-4" type="checkbox">
          </div>
          <hr>
          <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Price</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs text-gray-600">
            <p>Lowest</p>
            <p>Highest</p>
          </div>
          <div class="flex justify-between my-4 text-xs text-blue-500 font-bold">
            <p>Rp. 30.000,00</p>
            <p>Rp. 987.000,00</p>
          </div>
        </div>
      </div>
    </div>

    <button class="block md:hidden" @click="showModal">
      <svg class="h-8 w-8 text-gray-800" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4" />
      </svg>
    </button>

    <!-- ModalFilter -->
    <div class="bg-black bg-opacity-50 absolute inset-0 hidden justify-center items-center" id="filtermodal">
        <div class="container w-2/3 md:w-1/2 bg-white rounded-lg shadow-lg my-auto">
          <div class="px-6 py-4">
            <p class="text-right font-bold" @click="closeModal">X</p>
            <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Services</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>ANC</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>INC</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>PNC & BBL</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Contraseptive</p>
            <input class="mr-4" type="checkbox">
          </div>
          <hr>
          <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Midwife</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Jennifer</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Yasmin</p>
            <input class="mr-4" type="checkbox">
          </div>
          <div class="flex justify-between my-4 text-xs">
            <p>Bidan Yurike</p>
            <input class="mr-4" type="checkbox">
          </div>
          <hr>
          <div class="flex justify-between my-3 text-sm">
            <h4 class="font-bold">Price</h4>
            <Icons type='button-bottom'/>
          </div>
          <div class="flex justify-between my-4 text-xs text-gray-600">
            <p>Lowest</p>
            <p>Highest</p>
          </div>
          <div class="flex justify-between my-4 text-xs text-blue-500 font-bold">
            <p>Rp. 30.000,00</p>
            <p>Rp. 987.000,00</p>
          </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
import Swal from 'sweetalert2'

export default {
  methods: {
    showModal() {
      const overlay = document.querySelector('#filtermodal')
      overlay.classList.remove('hidden')
      overlay.classList.add('flex')
    },
    closeModal() {
      const close = document.querySelector('#filtermodal')
      close.classList.remove('flex')
      close.classList.add('hidden')
    }
  }
}
</script>
