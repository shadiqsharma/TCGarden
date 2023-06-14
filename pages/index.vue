<template>
  <div>
    <Header />
    <rooms />
    <facilities />

  </div>
</template>

<script>
import Facilities from "@/components/facilities/facilities";
import rooms from "@/components/rooms/rooms";
import Navbar from "@/components/Navbar/Navbar";

export default {
  name: 'IndexPage',
  components: {Navbar, Facilities, rooms},
}
</script>
