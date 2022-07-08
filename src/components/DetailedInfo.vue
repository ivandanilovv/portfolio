<template>
  <div class="pt-sm-4">
    <div class="row">
      <div class="col-12 col-md-9 text-start">
        <about-me class="py-2 border border-3 ps-3"/>
        <education class="pt-3 ps-3 mt-2 pt-md-2 border border-3"/>
        <experience class="pt-2 pt-md-2 ps-3 mt-2 border border-3"/>
      </div>
      <div class="col col-md-3 text-start">
        <skills class="pt-3 ps-3 mt-2 pt-md-2 ps-md-2 mt-md-0  border border-3"/>
        <languages class="py-3 px-3 my-2 px-md-1 border border-3"/>
        <rate class="py-3 px-3 my-2 px-md-1 border border-3"/>
      </div>
    </div>
  </div>
</template>

<script>
import Rate from "@/components/Rate";
import Skills from "@/components/Skills";
import AboutMe from "@/components/AboutMe";
import Education from "@/components/Education";
import Languages from "@/components/Languages";
import Experience from "@/components/Experience";


export default {
  name: "DetailedInfo",
  components: {
    Rate,
    Skills,
    AboutMe,
    Education,
    Languages,
    Experience
  }
}
</script>

<style scoped>

</style>