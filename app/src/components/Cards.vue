<template>
    <section class="py-0 lg:py-0 max-w-7xl mx-auto px-0 sm:px-8">
      <h2 class="text-4xl font-bold text-center mb-10">What We Do</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Card 1 -->
        <div class="w-full relative rounded-2xl overflow-hidden flex flex-col border-2">
          <img
            :src="image1"
            alt="Night Lights"
            class="w-full h-1/2 object-cover"
          />
          <div class="bg-secondary-color p-6 flex-grow rounded-b-2xl flex flex-col justify-between">
            <div>
              <h1 class="text-2xl font-semibold text-black">SPORTING ACTIVITIES</h1>
              <p class="text-black py-3">
                We offer a wide range of sporting activities designed to suit all ages and skill levels, ensuring there’s something for everyone. Whether you're a seasoned athlete or just looking to have fun, our diverse selection is tailored to meet your needs.
              </p>
            </div>
          </div>
        </div>
  
        <!-- Card 2 -->
        <div class="w-full relative rounded-2xl overflow-hidden flex flex-col border-2">
          <img
            :src="image2"
            alt="Welcome Aboard"
            class="w-full h-1/2 object-cover"
          />
          <div class="bg-secondary-color p-6 flex-grow rounded-b-2xl flex flex-col justify-between">
            <div>
              <h1 class="text-2xl font-semibold text-black">AGRICULTURAL ACTIVITIES</h1>
              <p class="text-black py-3">
                We offer a diverse range of agricultural activities that cater to enthusiasts, students, and families alike. Our programs and experiences aim to educate and engage participants in the world of farming and sustainable practices.
              </p>
            </div>
          </div>
        </div>
  
        <!-- Card 3 -->
        <div class="w-full relative rounded-2xl overflow-hidden flex flex-col border-2">
          <img
            :src="image3"
            alt="Welcome Aboard"
            class="w-full h-1/2 object-cover"
          />
          <div class="bg-secondary-color p-6 flex-grow rounded-b-2xl flex flex-col justify-between">
            <div>
              <h1 class="text-2xl font-semibold text-black">GRADUATION CEREMONIES</h1>
              <p class="text-black py-3">
                We specialize in creating exceptional graduation ceremonies that honor the achievements of students and provide a meaningful experience for all attendees. Our approach ensures that each ceremony is a unique celebration tailored to the needs and preferences of the graduating class.
              </p>
            </div>
          </div>
        </div>
  
        <!-- Card 4 -->
        <div class="w-full relative rounded-2xl overflow-hidden flex flex-col border-2">
          <img
            :src="image4"
            alt="Welcome Aboard"
            class="w-full h-1/2 object-cover"
          />
          <div class="bg-secondary-color p-6 flex-grow rounded-b-2xl flex flex-col justify-between">
            <div>
              <h1 class="text-2xl font-semibold text-black">CULTURAL ACTIVITIES</h1>
              <p class="text-black py-3">
                We offer a vibrant array of cultural activities designed to celebrate diversity, heritage, and artistic expression. Our programs aim to immerse participants in different cultures, encourage learning, and promote community engagement.
              </p>
            </div>
          </div>
        </div>
  
        <!-- Card 5 -->
        <div class="w-full relative rounded-2xl overflow-hidden flex flex-col border-2">
          <img
            :src="image5"
            alt="Welcome Aboard"
            class="w-full h-1/2 object-cover"
          />
          <div class="bg-secondary-color p-6 flex-grow rounded-b-2xl flex flex-col justify-between">
            <div>
              <h1 class="text-2xl font-semibold text-black">FASHION SHOW</h1>
              <p class="text-black py-3">
                We specialize in creating spectacular fashion shows that highlight the latest trends, celebrate creativity, and provide an unforgettable experience for all attendees. From concept to execution, our goal is to ensure a seamless and memorable event.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  import image1 from '../assets/017.jpg';
  import image2 from '../assets/fee 007.jpg';
  import image3 from '../assets/fee 239.jpg';
  import image4 from '../assets/439.jpg';
  import image5 from '../assets/fee 114.jpg';
  
  export default {
    data() {
      return {
        image1,
        image2,
        image3,
        image4,
        image5,
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add any component-specific styles here if needed */
  </style>
  