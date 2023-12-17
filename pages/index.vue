<template>
  <div>
    <Header />
    <div class="md:flex md:justify-between">
      <div class="my-12 lg:flex-row lg:items-center">
        <h4 class="flex lg:text-5xl text-3xl text-gray-800 justify-center mb-3">Empowering
          <p class="text-violet-500">&nbsp;Birthcare</p>
        </h4>
        <p class="flex lg:text-2xl text-lg text-gray-500 justify-center">Your Moments, Our Records.</p>
        <img src="../assets/img/jumbotronimage1.png" alt="jumbotron left" class="my-4 lg:max-w-xl">
      </div>
      <div>
        <img src="../assets/img/jumbotronimage2.png" alt="jumbotron right" class="lg:max-w-md hidden md:block">
      </div>
    </div>
    <div class="container pb-10">
      <b class="text-tracking mb-2">Services</b>
      <p class="font-bold text-xl mb-5">Our Services</p>
      <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-5 justify-items-center mb-20">
        <nuxt-link to="/">
          <img src="../assets/img/ANC.png" alt="trending" class="image-trending rounded-3xl lg:w-52">
        </nuxt-link>
        <nuxt-link to="/">
          <img src="../assets/img/INC.png" alt="trending" class="image-trending rounded-3xl lg:w-52">
        </nuxt-link>
        <nuxt-link to="/">
          <img src="../assets/img/PNC.png" alt="trending" class="image-trending rounded-3xl lg:w-52">
        </nuxt-link>
        <nuxt-link to="/">
          <img src="../assets/img/KB.png" alt="trending" class="image-trending flex lg:w-52 md:hidden lg:flex rounded-3xl">
        </nuxt-link>
      </div>
      <CardTrending />
    </div>
    <Footer />
  </div>
</template>
