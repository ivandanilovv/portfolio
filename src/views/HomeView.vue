<template>
  <main class="container py-5">
    <bio/>
    <div class="pt-sm-4 pt-md-4">
      <div class="row">
        <div class="col-12 col-md-9 text-start">
          <about-me class="pt-3 pt-md-0"/>
          <education class="pt-3"/>
        </div>
        <div class="col text-start">
          <skills class="pt-3 pt-md-0"/>
          <languages class="pt-3"/>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
// @ is an alias to /src
import Bio from "@/components/Bio";
import Skills from "@/components/Skills";
import AboutMe from "@/components/AboutMe";
import Languages from "@/components/Languages";
import Education from "@/components/Education";

export default {
  name: 'HomeView',
  components: {
    Bio,
    Skills,
    AboutMe,
    Languages,
    Education
  }
}
</script>
<style scoped>

</style>
