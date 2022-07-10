<template>
  <div class="pt-sm-4">
    <div class="row">
      <div class="col-12 col-md-8 text-start">
        <about-me class="py-2 ps-3 mt-sm-0 mt-3 custom-border"/>
        <education class="pt-3 ps-3 pt-md-2 mt-2 custom-border"/>
        <experience class="pt-2 pt-md-2 ps-3 mt-2 custom-border"/>
      </div>
      <div class="col col-md-4 text-start">
        <skills class="pt-3 ps-3 pt-md-2 ps-md-2 mt-2 mt-md-0 custom-border"/>
        <languages class="py-2 px-3 px-md-1 my-2 custom-border"/>
        <achievements class="py-2 px-3 pt-3 px-md-1 my-2 custom-border"/>
        <rate class="py-3 px-3 px-md-1 my-2 custom-border"/>
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
import Achievements from "@/components/Achievements";


export default {
  name: "DetailedInfo",
  components: {
    Achievements,
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
.custom-border{
  border: 3px solid #b84646;
}
</style>