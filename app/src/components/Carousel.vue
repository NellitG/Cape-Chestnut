<template>
    <!-- First Section: Content on the left, Image on the right with added spacing -->
    <div class="max-w-screen-xl px-4 py-12 mx-auto lg:gap-8 xl:gap-0 lg:py-0 lg:grid lg:grid-cols-12 my-12">
      <div class="lg:col-span-6 place-self-center lg:pr-8"> <!-- Added lg:pr-8 -->
        <h1 class="max-w-2xl mb-4 text-3xl font-semibold md:text-5xl xl:text-6xl">
          Our Environment
        </h1>
        <p class="max-w-2xl sm:mt-10 font-semibold text-gray-950 lg:mb-8 md:text-lg lg:text-xl">
          Cape Chestnut School is nestled in a beautiful, scenic environment that enhances the learning experience for our students.
          Surrounded by lush greenery and vibrant Cape Chestnut trees, the school offers a peaceful and inspiring setting for both study and play.
        </p>
      </div>
      <div class="lg:col-span-6 lg:flex justify-center lg:pl-8"> <!-- Added lg:pl-8 -->
        <img src="@/assets/garden.jpg" alt="Garden Image" />
      </div>
    </div>
  
    <!-- Second Section: Image on the left, Content on the right with added spacing -->
    <div class="max-w-screen-xl px-4 py-12 mx-auto lg:gap-8 xl:gap-0 lg:py-0 lg:grid lg:grid-cols-12 my-12">
      <div class="lg:col-span-6 lg:flex justify-center lg:pr-8"> <!-- Added lg:pr-8 -->
        <img src="@/assets/chestnut.jpg" alt="Chestnut Tree Image" />
      </div>
      <div class="lg:col-span-6 place-self-center lg:pl-8"> <!-- Added lg:pl-8 -->
        <h2 class="max-w-2xl mb-4 text-2xl font-semibold md:text-4xl xl:text-5xl">
          The Garden Area
        </h2>
        <p class="max-w-2xl sm:mt-10 font-semibold text-gray-950 lg:mb-8 md:text-lg lg:text-xl">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar dapibus leo.
        </p>
      </div>
    </div>
  
    <!-- Third Section: Content on the left, Image on the right with added spacing -->
    <div class="max-w-screen-xl px-4 py-12 mx-auto lg:gap-8 xl:gap-0 lg:py-0 lg:grid lg:grid-cols-12 my-12">
      <div class="lg:col-span-6 place-self-center lg:pr-8"> <!-- Added lg:pr-8 -->
        <h2 class="max-w-2xl mb-4 text-2xl font-semibold md:text-4xl xl:text-5xl">
          The Tree Grove
        </h2>
        <p class="max-w-2xl sm:mt-10 font-semibold text-gray-950 lg:mb-8 md:text-lg lg:text-xl">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar dapibus leo.
        </p>
      </div>
      <div class="lg:col-span-6 lg:flex justify-center lg:pl-8"> <!-- Added lg:pl-8 -->
        <img src="@/assets/trees.jpg" alt="Trees Image" />
      </div>
    </div>
  </template>
  