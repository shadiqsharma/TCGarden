<template>
  <div class="relative flex items-center justify-between w-full h-20 px-8 ">
    <a href="#_" class="relative flex items-center h-full pr-6 ">
      <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686569834/TC/TC_Garden_White_meecmy.png" alt="tcgarden_logo" class="h-20">
      <span class="text-blue-700">.</span>
    </a>
    <nav
      class="top-0 left-0 flex-col items-center justify-center hidden h-full space-y-3 bg-white md:justify-end md:bg-transparent md:space-x-5 md:space-y-0 md:relative md:flex md:flex-row"
      :class="{'flex fixed top-0 left-0 w-full z-40': showMenu, 'hidden': !showMenu }"
    >
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm md:text-white">
        <span class="block">Home</span>
      </a>
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">Rooms</span>
      </a>
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">Attraction</span>
      </a>
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">Promotions</span>
      </a>
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm">
        <span class="block">About Us</span>
      </a>
      <a href="#_" class="relative text-lg font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm md:text-white">
        <span class="block">Contact</span>
      </a>

    </nav>

    <!-- Mobile Nav -->
    <nav class="fixed top-0 right-0 z-30 z-50 flex w-10 h-10 mt-4 mr-4 md:hidden">
      <button @click="showMenu = !showMenu" class="flex items-center justify-center w-10 h-10 rounded-full hover:bg-white hover:bg-opacity-25 focus:outline-none">
        <svg class="w-5 h-5 text-gray-200 fill-current" v-show="!showMenu" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
          <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
        </svg>
      </button>
      <ul v-show="showMenu" class="fixed top-0 left-0 w-screen h-screen bg-black bg-opacity-80 z-50 flex flex-col justify-center items-center">
        <li class="mb-4">
          <a href="#_" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-sm text-white">
            <span class="block">Home</span>
          </a>
        </li>
        <li class="mb-4">
          <a href="#_" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
            <span class="block">Rooms</span>
          </a>
        </li>
        <li class="mb-4">
          <a href="#" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
            <span class="block">Attraction</span>
          </a>
        </li>
        <li class="mb-4">
          <a href="#_" class="relative text-xl font-medium tracking-wide text-blue-700 transition duration-150 ease-out md:text-white md:text-sm text-white">
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
    </nav>


    <!-- End Mobile Nav -->
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      showMenu: false,
    };
  },
};
</script>

