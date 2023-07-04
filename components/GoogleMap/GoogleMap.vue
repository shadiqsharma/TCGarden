<template>
  <div style="width: 100%">
    <iframe class="rounded-2xl"
      width="100%"
      height="600"
      frameborder="0"
      scrolling="no"
      marginheight="0"
      marginwidth="0"
      :src="googleMapsUrl">
      <a href="https://www.maps.ie/distance-area-calculator.html">measure distance on map</a>
    </iframe>
  </div>
</template>

<script>
export default {
  name: 'GoogleMap',
  data() {
    return {
      googleMapsUrl: 'https://maps.google.com/maps?width=100%25&height=600&hl=en&q=tc%20garden%20resort+(TC%20Garden%20Resort)&t=&z=14&ie=UTF8&iwloc=B&output=embed',
    };
  },
};
</script>

<style scoped>
iframe {
  border: 0;
}
</style>
