<template>
  <main class="container pt-5 bg-color">
    <bio :contact-info="contactInfo" :contact-links="contactLinks"/>
    <detailed-info/>
    <hr/>
    <my-footer/>
  </main>
</template>

<script>
// @ is an alias to /src
import Bio from "@/components/Bio";
import DetailedInfo from "@/components/DetailedInfo";
import MyFooter from "@/components/MyFooter";

export default {
  name: 'HomeView',
  components: {
    MyFooter,
    Bio,
    DetailedInfo
  },
  data() {
    return {
      contactLinks: [
        {
          fontAwesomeLogo: 'fs-4 pe-2 fa fa-linkedin-square font-awesome-color',
          text: 'http://www.linkedin.com/in/ivandanilov1'
        },
        {
          fontAwesomeLogo: 'fs-4 pe-2 fa fa-github font-awesome-color',
          text: 'https://github.com/ivandanilovv'
        }
        ],
      contactInfo: [
        {
          fontAwesomeLogo: 'fs-5 pe-2 fa fa-phone-square font-awesome-color',
          text: '+389 70296123'
        },
        {
          fontAwesomeLogo: 'fs-4 pe-3 fa fa-map-marker font-awesome-color',
          text: 'Cyril and Methodius 60, 2300, Kocani(Macedonia)'
        },
        {
          fontAwesomeLogo: 'fs-5 pe-2 fa fa-envelope font-awesome-color',
          text: 'ivandanilov282@gmail.com'
        }
        ],
    }
  }
}
</script>
<style scoped>
.bg-color{
  background-color: #d7dde4;
}
</style>
