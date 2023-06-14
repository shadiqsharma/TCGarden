<template>
  <section class="py-10 bg-gray-50 overflow-hidden">
    <div class="container mx-auto px-4">
      <div class="py-16 px-8 bg-white rounded-3xl shadow-sm">
        <div class="mb-12 md:max-w-4xl mx-auto text-center">
          <h2 class="font-heading mb-6 text-4xl md:text-5xl lg:text-6xl text-gray-900 font-black tracking-tight">Deluxe King Villa</h2>
        </div>
    <carousel :responsive="{0:{items:1,nav:false},600:{items:2,nav:false},1024:{items:3,nav:false}}"
              class="w-auto h-auto">
      <div class="container px-2">
        <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686572325/TC/luxury-resort-hotel-room-2022-11-14-06-58-44-utc_apcjas.jpg" class="w-full h-72 object-cover rounded-2xl">
        <p class="text-center px-2 py-4">Bedroom</p>
      </div>
      <div class="container px-2">
        <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686572064/TC/TCFront_dezovr.webp" class="w-full h-72 object-cover rounded-2xl">
        <p class="text-center px-2 py-4">Bathroom</p>
      </div>
      <div class="container px-2">
        <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1686572038/TC/TCG_room2_qjfe3b.jpg" class="w-full h-72 object-cover rounded-2xl">
        <p class="text-center px-2 py-4">Garden</p>
      </div>
    </carousel>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'castCarousel'
}
</script>

<style scoped>
</style>
