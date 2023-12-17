<template>
  <div>
    <Header type='home'/>
    <div class="bg-gray-200 py-10">
      <div class="container block md:flex gap-10">
        <CardProfile />
        <div class="w-full bg-white rounded-lg shadow-lg mt-10 md:mt-0">
          <div class="px-6 py-4">
            <div>
              <b class="text-xs text-blue-600 tracking-widest uppercase mb-2">Profile</b>
              <p class="font-bold text-2xl mb-2">Profile</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 text-sm">
              <!-- left -->
              <div class="my-3">
                <b>Contact</b>
                <p class="text-description-sm">Email</p>
                <input class="input-form" type="email" placeholder="midwife@matrilog.com">
                <p class="text-description-sm">Phone Number</p>
                <input class="input-form" type="number" placeholder="+62 78237595">
                <div class="flex justify-end">
                  <b class="text-blue-600">
                    Account Settings
                  </b>
                </div>
              </div>
              <!-- Right -->
              <div class="my-3">
                <b>Biodata</b>
                <p class="text-description-sm">Username</p>
                <input class="input-form" type="text" placeholder="Nadine Kowalski">
                <p class="text-description-sm">City</p>
                <select class="input-form">
                  <option selected disabled>Medan</option>
                  <option selected disabled>Bogor</option>
                </select>
                <p class="text-description-sm">Address</p>
                <input class="input-form" type="text" placeholder="Medan, Indonesia">
                <p class="text-description-sm">STR</p>
                <input class="input-form" type="text" placeholder="55555">
                <button @click="update" class="btn-auth mt-8">Save</button>
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
import Swal from 'sweetalert2'

export default {
  name: 'UpdateProfile',
  methods: {
    update() {
      Swal.fire(
        'Update',
        'Your Profile Saved',
        'success'
      )
      this.$router.push('/profile')
    }
  }
}
</script>
