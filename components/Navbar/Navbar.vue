<template>
  <div>
  <div class="fixed w-full z-50 flex items-center justify-between h-20 px-8 bg-yellow-800 bg-opacity-50">
    <a href="/" class="relative flex items-center h-full pr-6 ">
      <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686569834/TC/TC_Garden_White_meecmy.png" alt="tcgarden_logo" class="h-20">
    </a>

    <nav
      class="top-0 left-0 flex-col items-center justify-center hidden h-full space-y-3 bg-white md:justify-end md:bg-transparent md:space-x-5 md:space-y-0 md:relative md:flex md:flex-row"
      :class="{'flex fixed top-0 left-0 w-full z-40': showMenu, 'hidden': !showMenu }"
    >
      <nuxt-link to="/" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm md:text-white">
        <span class="block">Home</span>
      </nuxt-link>

      <a href="#"
         @click.prevent="toggleSubMenu('Rooms')"
         class="relative text-lg font-medium
   tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">Rooms</span>

        <div v-if="activeSubMenu === 'Rooms'"
             class="absolute left-0 mt-2 w-48 rounded-md shadow-lg bg-white z-50">
          <div class="py-1 rounded-md bg-white shadow-xs">
            <nuxt-link to="/deluxeking" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">Deluxe King Villa</nuxt-link>
            <nuxt-link to="/deluxetriple" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">Deluxe Triple Villa</nuxt-link>
            <nuxt-link to="/" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">Deluxe Quad Villa</nuxt-link>
          </div>
        </div>
      </a>
      <nuxt-link to="/" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">Attraction</span>
      </nuxt-link>

      <nuxt-link to="/about" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">About Us</span>
      </nuxt-link>
      <nuxt-link to="/" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm md:text-white">
        <span class="block">Contact Us</span>
      </nuxt-link>

    </nav>

    <!-- Mobile Nav -->
    <div class="fixed top-0 right-0 z-30 z-50 flex w-10 h-10 mt-4 mr-4 md:hidden">
      <button @click="showMenu = !showMenu" class="flex items-center justify-center w-10 h-10 rounded-full hover:bg-white hover:bg-opacity-25 focus:outline-none">
        <svg class="w-5 h-5 text-gray-200 fill-current" v-show="!showMenu" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
          <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
        </svg>
      </button>
      <ul v-show="showMenu" class="fixed top-0 left-0 w-screen h-screen bg-black bg-opacity-90 z-50 flex flex-col justify-center items-center">
        <li class="mb-4">
          <nuxt-link to="/" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm text-white">
            <span class="block">Home</span>
          </nuxt-link>
        </li>
        <li class="mb-4">
          <a href="#"
             @click.prevent="toggleSubMenu('Rooms')"
             class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
            <span class="block">Rooms</span>

            <div v-if="activeSubMenu === 'Rooms'"
                 class="absolute left-0 mt-2 w-48 rounded-md shadow-lg bg-white z-50">
              <div class="py-1 rounded-md bg-white shadow-xs">
                <nuxt-link to="/deluxeking" @click.native.prevent="closeMenu" class="block px-4 py-2 text-sm text-gray-700 hover:bg-yellow-500">Deluxe King Villa</nuxt-link>
                <nuxt-link to="/deluxetriple" @click.native.prevent="closeMenu" class="block px-4 py-2 text-sm text-gray-700 hover:bg-yellow-500">Deluxe Triple Villa</nuxt-link>
                <nuxt-link to="/" @click.native.prevent="closeMenu" class="block px-4 py-2 text-sm text-gray-700 hover:bg-yellow-500">Deluxe Quad Villa</nuxt-link>
              </div>
            </div>
          </a>
        </li>

        <li class="mb-4">
          <a href="#" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
            <span class="block">Attraction</span>
          </a>
        </li>
        <li class="mb-4">
          <a href="/about" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
            <span class="block">About Us</span>
          </a>
        </li>
        <li class="mb-4">
          <a href="#_" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm text-white">
            <span class="block">Contact</span>
          </a>
        </li>
        <li>
          <button @click="showMenu = !showMenu" class="absolute top-3 right-3 focus:outline-none">
            <svg class="w-10 h-10 text-gray-100 fill-current" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path d="M13.41 12l3.29-3.29a1 1 0 0 0-1.42-1.42L12 10.59l-3.29-3.3a1 1 0 1 0-1.42 1.42L10.59 12l-3.3 3.29a1 1 0 0 0 1.42 1.42L12 13.41l3.29 3.3a1 1 0 0 0 1.42-1.42L13.41 12z"></path>
            </svg>
          </button>
        </li>
      </ul>
    </div>


    <!-- End Mobile Nav -->
  </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      showMenu: false,
      activeSubMenu: null,
    };
  },
  methods: {
    toggleSubMenu(menuName) {
      if (this.activeSubMenu === menuName) {
        this.activeSubMenu = null;
      } else {
        this.activeSubMenu = menuName;
      }
    },
    closeMenu() {
      this.showMenu = false;

    }
  }
};
</script>

