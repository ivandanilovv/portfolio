<template>
  <main class="container py-5">
    <bio/>
    <detailed-info/>
  </main>
</template>

<script>
// @ is an alias to /src
import Bio from "@/components/Bio";
import DetailedInfo from "@/components/DetailedInfo";

export default {
  name: 'HomeView',
  components: {
    Bio,
    DetailedInfo
  }
}
</script>
<style scoped>

</style>
