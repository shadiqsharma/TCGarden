<template>
  <div>
    <Header />
    <rooms />
    <facilities />
  <!-- Create Promotion Pop Up Here   -->
    <!--    <popup/> -->
  </div>
</template>

<script>
import Facilities from "@/components/facilities/facilities";
import rooms from "@/components/rooms/rooms";
import Navbar from "@/components/Navbar/Navbar";
import Popup from "@/components/popup/popup";

export default {
  name: 'IndexPage',
  components: {Popup, Navbar, Facilities, rooms},
}
</script>
