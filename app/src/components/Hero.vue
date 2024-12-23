<template>
    <div class="relative w-full h-screen flex items-center justify-center">
      <img
        :src="feeImage"
        alt="bg-img"
        class="absolute inset-0 w-full h-full object-cover"
      />
  
      <div class="container mx-auto relative z-10 mt-24 py-10">
        <div class="grid grid-cols-12 text-center lg:text-start">
          <div
            class="relative flex flex-col bg-clip-border lg:ml-20 text-gray-700 px-16 py-0 border border-white shadow-lg col-span-full rounded-xl bg-transparent shadow-black/10 backdrop-blur-sm backdrop-saturate-200 xl:col-span-8"
          >
            <h1
              class="tracking-normal font-semibold text-white lg:text-white text-5xl !leading-snug lg:text-6xl"
            >
              Cape Chestnut School
            </h1>
            <p
              class="antialiased font-sans text-2xl font-semibold leading-relaxed text-inherit mb-10 mt-6 text-white lg:text-white"
            >
              Good Education, Good Character
            </p>
            <div class="flex justify-center gap-4 mb-8 lg:justify-start">
              <router-link to="/contact">
                <button
                  class="align-middle select-none font-sans font-semibold text-center uppercase transition-all disabled:opacity-50 disabled:shadow-none disabled:pointer-events-none text-xs py-3 px-6 rounded-lg hover:bg-green-500 text-white sm:text-white border-2 border-green-500 shadow-md shadow-primary-color/10 hover:shadow-lg hover:shadow-primary-color/10 focus:opacity-[0.85] focus:shadow-none active:opacity-[0.85] active:shadow-none"
                  type="button"
                >
                  contact us
                </button>
              </router-link>
              <router-link to="/academics">
                <button
                  class="align-middle select-none font-semibold text-center lg:text-white uppercase transition-all disabled:opacity-50 disabled:shadow-none disabled:pointer-events-none text-xs py-3 px-6 rounded-lg border-green-500 border-2 hover:bg-green-500 text-white hover:opacity-75 focus:ring focus:ring-gray-300 active:opacity-[0.85]"
                  type="button"
                >
                  read more
                </button>
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import feeImage from '../assets/fee 237.jpg'; // Ensure this path is correct
  
  export default {
    data() {
      return {
        feeImage, // Use the imported image in the template
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add any component-specific styles here if needed */
  </style>
  