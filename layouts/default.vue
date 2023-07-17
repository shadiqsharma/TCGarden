<template>
  <div>
    <Navbar />
    <nuxt/>
    <Footer/>
  </div>
</template>
<script>

import Footer from "@/components/footer/footer";
export default {
  head: {
    script: [
      {
        src: '/gtag-init.js',
        async: true,
        defer: true
      }
    ]
  },
  components: {Footer}
}
</script>
