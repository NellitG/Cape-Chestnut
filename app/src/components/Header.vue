<template>
  <div>
    <!-- Header section -->
    <header
      :class="{
        'h-14 lg:h-36 fixed w-full top-0 inset-0 z-20 bg-white': isHomePage,
        'h-14 lg:h-24 fixed w-full top-0 inset-0 z-20 bg-white': !isHomePage,
      }"
    >
    
      <div
        class="flex items-center justify-between mx-auto max-w-7xl h-full px-4 lg:px-0"
      >
        <!-- Logo and menu toggle button -->
        <div class="flex items-center gap-6">
          <button
            class="text-2xl p-1 text-black hover:text-blue-500 lg:hidden"
            @click="toggleMenu2"
          >
            {{ close2 ? "☰" : "✘" }}
          </button>
          <router-link
            to="/"
            class="flex items-center"
            @click.native="closeMenu"
          >
            <img
              src="@/assets/cape-chestnut.png"
              alt="Logo"
              class="h-8 lg:h-28 mb-0 mt-6 ml-12"
            />
          </router-link>
        </div>

        <!-- Navigation menu -->
        <nav
          :class="{ hidden: close2, flex: !close2 }"
          class="bg-black lg:bg-white lg:static lg:flex lg:items-center flex-1 justify-center absolute top-14 lg:top-0 left-0 w-full lg:w-auto"
        >
          <!-- Navigation items -->
          <ul
            class="flex flex-col lg:flex-row gap-6 lg:gap-8 text-white lg:text-black mt-4 lg:mt-0 lg:items-center px-4 lg:px-0"
          >
            <li>
              <router-link
                to="/"
                class="hover:text-green-500"
                active-class="hover:text-green-500"
                @click.native="closeMenu"
                >Home</router-link
              >
            </li>
            <li class="relative group">
              <router-link
                to="/academics"
                class="hover:text-green-500 flex items-center"
                active-class="hover:text-green-500"
                @click.native="closeMenu"
              >
                <span>Academics</span>
                <span class="ml-1"></span>
              </router-link>
            
            </li>
            <li>
              <router-link
                to="/aboutus"
                class="hover:text-green-500"
                active-class="hover:text-fuchsia-500"
                @click.native="closeMenu"
                >About Us</router-link
              >
            </li>
          
            <li>
              <router-link
                to="/contact"
                class="hover:text-green-500"
                active-class="hover:text-green-500"
                @click.native="closeMenu"
                >Contact Us</router-link
              >
            </li>
            <li>
              <router-link
                to="/admission"
                class="hover:text-green-500 relative"
                active-class="hover:text-green-500"
                @click.native="closeMenu"
              >
                Admission
               
              </router-link>
            </li>
          </ul>
        </nav>
      </div>
    </header>
  </div>
</template>

<script>
// import logo from '../assets/cape-chestnut.png';
export default {
  data() {
    return {
      close2: true,
    };
  },
  computed: {
    isHomePage() {
      return this.$route.path === "/";
    },
  },
  watch: {
    $route(to, from) {
      if (to.path === "/") {
        this.close2 = true;
      }
    },
  },
  methods: {
    toggleMenu2() {
      this.close2 = !this.close2;
    },
    closeMenu() {
      this.close2 = true;
    },
  },
  mounted() {
    if (this.isHomePage) {
      this.close2 = true;
    }
  },
};
</script>

<style scoped>
button {
  font-size: 2rem;
}
</style>
