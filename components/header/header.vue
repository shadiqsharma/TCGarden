<template xmlns="http://www.w3.org/1999/html">
    <div>
      <section class="relative w-screen h-screen bg-top bg-cover md:bg-center" style="background-image:url('https://res.cloudinary.com/dgsljij3o/image/upload/v1686398741/TC/palm-tree-in-tropical-garden-2022-12-29-02-40-50-utc_1_vypze0.jpg')">
        <div class="absolute inset-0 w-full h-full bg-gray-900 opacity-25"></div>
        <div class="absolute inset-0 w-full h-64 opacity-50 bg-gradient-to-b from-black to-transparent"></div>
<!--        Navbar -->
        <div class="relative z-10 max-w-6xl px-10 py-40 mx-auto">
          <div class="flex flex-col items-center h-full lg:flex-row">
            <div class="flex flex-col items-center justify-center w-full h-full lg:w-2/3 lg:items-start">

              <h1 class="font-extrabold tracking-tight text-center text-white text-3xl lg:text-left xl:pr-32"><a href="#_" class="relative flex items-center h-full pr-6 ">
                <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686569834/TC/TC_Garden_White_meecmy.png" alt="tcgarden_logo" class="h-20">
              </a></h1>
              <h1 class="font-extrabold tracking-tight text-center text-white text-7xl lg:text-left xl:pr-32">TC GARDEN RESORT</h1><br/>

              <div class="w-auto md:w-auto p-2"><a class="block w-full px-12 py-3.5 text-lg text-center text-white font-bold bg-yellow-500 hover:bg-yellow-600 focus:ring-4 focus:ring-gray-600 rounded-md" href="#">Book Now</a></div>
            </div>
            <div class=" items-center justify-center w-full h-full max-w-sm mt-20 lg:mt-0 lg:w-1/3 ">

            </div>
          </div>
        </div>

      </section>
    </div>
</template>

<script>
    export default {
        name: 'Header',
      data() {
        return {
          showMenu: false,
          // other reactive properties...
        }
      }
    }
</script>

<style>
.custom-menu {
  width: 120px; /* Customize the width as per your preference */
}
</style>
