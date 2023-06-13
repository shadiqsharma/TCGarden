<template>
  <div>
    <Header />
    <rooms/>
    <facilities />
  </div>
</template>

<script>
import Facilities from "@/components/facilities/facilities";
export default {
  name: 'IndexPage',
  components: {Facilities},
}
</script>
