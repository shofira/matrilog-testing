<template>
  <div>
    <div class="flex">
      <div class="w-3/5 bg-violet-500 h-screen hidden sm:flex">
        <img src="../assets/img/illustrationbackground.png" class="m-auto md:max-w-sm">
      </div>
      <div class="w-full md:w-2/5 h-screen p-8 md:p-10">
        <div class="hidden sm:flex">
          <img src="../assets/img/logomatrilog.png" class="inline w-11 mr-2 mb-2" alt="logo matrilog">
          <b class="text-xl text-gray-700 tracking-wider">Matrilog</b>
        </div>
        <nuxt-link to="/splashscreen" class="flex sm:hidden">
          <Icons type="button-back" />
        </nuxt-link>

        <form class="mt-8 lg:mt-12">
          <b class="text-2xl text-gray-800">Login</b>
          <div class="mt-10 mb-4">
            <input class="input-form" type="text" placeholder="Username" required>
          </div>
          <div class="mb-3">
            <input class="input-form" type="password" placeholder="Password" required>
          </div>
          <button class="btn-auth" @click="login">
            Sign In
          </button>
          <div class="text-center mt-3 leading-6">
            <p class="text-gray-600 text-sm">Did you forgot your password?</p>
            <a class="text-right text-sm text-violet-500 hover:text-violet-700 cursor-pointer" @click="showModal()">
              Tap here for reset
            </a>
            <hr class="mt-3">
            <p class="text-sm text-gray-600 mt-3 mb-2">Or sign in with</p>
            <div class="flex items-center justify-center space-x-4 mb-4">
              <button class="btn-outline-auth" disabled>
                <img src="../assets/img/google.png" alt="google sign in">
              </button>
              <button class="btn-outline-auth" disabled>
                <img src="../assets/img/fb.png" alt="facebook sign in">
              </button>
            </div>
            <p class="text-sm text-gray-700">
              Dont Have an account?
              <nuxt-link to="/register" class=" text-violet-500 hover:text-blue-700 cursor-pointer">Please, create a new one</nuxt-link>
            </p>
          </div>
        </form>
      </div>
    </div>

    <!-- ModalForgot -->
    <div class="bg-black bg-opacity-50 absolute inset-0 hidden justify-center items-center" id="modalForgot">
      <div class="bg-white text-center max-w-md p-5 mx-5 rounded-lg">
        <div class="mb-10 flex justify-between items-center">
          <p class="text-xl tracking-wider">
            <img src="../assets/img/logomatrilog.png" class="w-10 mr-2 inline" alt="logo matrilog">
            Matrilog
          </p>
          <svg class="h-5 w-5" @click="closeModal" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </div>
        <p class="text-description">
          Forgot your password?
          Please, enter your email here! You'll get message soon to create a new password
        </p>
        <input class="w-full border border-gray-500 rounded w-2/3 py-2 px-4 my-4 focus:outline-none focus:border-blue-500" type="email" placeholder="email@gmail.com" required>
        <button class="btn-auth" @click="sendMailForgot">Send</button>
      </div>
    </div>
  </div>
</template>

<script>
import Swal from 'sweetalert2'

export default {
  methods: {
    showModal() {
      const overlay = document.querySelector('#modalForgot')
      overlay.classList.remove('hidden')
      overlay.classList.add('flex')
    },
    closeModal() {
      const close = document.querySelector('#modalForgot')
      close.classList.remove('flex')
      close.classList.add('hidden')
    },
    sendMailForgot() {
      Swal.fire(
        'Success',
        'Please check your email to reset password',
        'success'
      )
      this.closeModal()
    },
    login() {
      this.$router.push('/')
    }
  }
}
</script>
