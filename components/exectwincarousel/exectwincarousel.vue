<template>
  <section class="py-10 bg-gray-50 overflow-hidden">
    <div class="container mx-auto px-4">
      <div class="py-16 px-8 bg-white rounded-3xl shadow-sm">
        <div class="mb-12 md:max-w-4xl mx-auto text-center">
          <h2 class="font-heading mb-6 text-4xl md:text-5xl lg:text-6xl text-gray-900 font-black tracking-tight">Executive Twin Villa</h2>
        </div>
        <carousel :responsive="{0:{items:1,nav:false},600:{items:2,nav:false},1024:{items:3,nav:false}}"
                  class="w-auto h-auto">
          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1688205150/TC/executive%20twin/photo_2023-06-26_20-55-25_yyvxjm.webp" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Bedroom</p>
          </div>
          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1688205150/TC/executive%20twin/photo_2023-06-26_20-55-33_jgrdwh.webp" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Bed View</p>
          </div>
          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1688205150/TC/executive%20twin/photo_2023-06-26_20-55-39_siiuyf.webp" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Room Plan</p>
          </div>
          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1688205150/TC/executive%20twin/photo_2023-06-26_20-55-42_ghvtvy.webp" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Bed View</p>
          </div>
          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1687524716/TC/deluxe%20king%20rooom/IMG_2040_kqoyxz.jpg" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Toilet</p>
          </div>

          <div class="container px-2">
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1687524719/TC/deluxe%20king%20rooom/IMG_2051_cgjwyp.jpg" class="w-full h-72 object-cover rounded-2xl">
            <p class="text-center px-2 py-4">Front View</p>
          </div>
        </carousel>
      </div>

    </div>
  </section>
</template>
<script>
export default {
  name: 'Exectwincarousel'
};
</script>

<style scoped>
</style>



