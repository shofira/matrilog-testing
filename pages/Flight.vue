<template>
  <div>
    <Header type='home'/>
    <div class="bg-gray-200 pb-10">
      <div class="bg-violet-500 rounded-b-3xl flex items-center">
        <h1 class="text-violet-500 text-8xl">asdf</h1>
      </div>
      <div class="container block md:flex gap-10">
        <div class="w-1/2">
          <FilterBox />
        </div>
        <div class="w-full">
          <CardFlight />
        </div>
      </div>
    </div>
    <Footer/>
  </div>
</template>
