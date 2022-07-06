<template>
  <div class="pt-sm-4 pt-md-4">
    <div class="row">
      <div class="col-12 col-md-9 text-start">
        <about-me class="pt-3 pt-md-0"/>
        <education class="pt-3"/>
        <experience class="pt-3"/>
      </div>
      <div class="col text-start">
        <skills class="pt-3 pt-md-0"/>
        <languages class="pt-3"/>
      </div>
    </div>
  </div>
</template>

<script>
import Skills from "@/components/Skills";
import AboutMe from "@/components/AboutMe";
import Education from "@/components/Education";
import Languages from "@/components/Languages";
import Experience from "@/components/Experience";

export default {
  name: "DetailedInfo",
  components: {
    Experience,
    Skills,
    AboutMe,
    Education,
    Languages
  }
}
</script>

<style scoped>

</style>