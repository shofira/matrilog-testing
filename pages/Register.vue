<template>
  <div>
    <div class="flex">
      <div class="w-3/5 bg-violet-500 h-screen hidden sm:flex">
        <img src="../assets/img/illustrationbackground.png" class="m-auto md:max-w-sm">
      </div>
      <div class="w-full md:w-2/5 h-screen p-8 md:p-10">
        <div class="hidden sm:flex">
          <img src="../assets/img/logomatrilog.png" class="inline w-10 mb-2" alt="logo matrilog">
          <b class="text-xl text-gray-700 tracking-wider">Matrilog</b>
        </div>
        <div class="flex sm:hidden flex justify-between">
          <nuxt-link to="/splashscreen" class="inline">
            <Icons type="button-back" />
          </nuxt-link>
          <a class="text-violet-400 text-sm text-right cursor-pointer">Continue as Guest</a>
        </div>

        <form class="mt-8 lg:mt-16 space-y-3">
          <b class="text-2xl text-gray-800">Register</b>
          <div class="mt-10">
            <input class="input-form" type="text" placeholder="Fullname" required>
          </div>
          <div>
            <input class="input-form" type="email" placeholder="Email@gmail.com" required>
          </div>
          <div>
            <input class="input-form" type="password" placeholder="Password" required>
          </div>
          <button @click="register" class="btn-auth">
            Sign Up
          </button>
          <label class="block mt-3 text-gray-600">
            <input class="mr-2" type="checkbox" required>
            <span class="text-description">
              Accept terms and condition!
            </span>
          </label>
          <div class="text-center mt-3 leading-6">
            <hr>
            <p class="text-description">Already have an account?</p>
            <div class="flex items-center justify-center">
              <nuxt-link to="/login" class="w-full btn-outline-auth">
                Sign In
              </nuxt-link>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import Swal from 'sweetalert2'

export default {
  name: 'Login',
  methods: {
    register() {
      Swal.fire(
        'Your Registration Success',
        'Please Check Your Email to activate',
        'success'
      )
      this.$router.push('/login')
    }
  }
}
</script>
