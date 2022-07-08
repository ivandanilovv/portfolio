<template>
  <section>
    <div class="row text-start">
      <div class="col-2 d-flex flex-column justify-content-center">
        <div class="ratio ratio-2x3">
          <img src="../assets/images/tablo_resized.jpg" alt="Profle image">
        </div>
      </div>
      <div class="col-10 col-md-3 align-bottom d-flex flex-column justify-content-center">
        <h2 class="fw-bold headings-color">
          Ivan Danilov
        </h2>
        <h4 class="job-title-color">
          Full Stack Developer
        </h4>
      </div>
      <div class="col-12 col-md-5 text-start d-flex flex-column justify-content-center ps-3 ">
        <h3 class="fw-bold headings-color pt-3 pt-md-0">
          Contact
        </h3>
        <div v-for="contact in contactInfo">
          <div class="d-flex flex-row info-font-size align-items-center">
            <div class="d-flex justify-content-center font-awesome-scale">
              <i class="font-awesome-rotate" :class="[contact.fontAwesomeLogo]" aria-hidden="true"
                 @mouseover="hover = true"></i>
            </div>
            {{ contact.text }}
          </div>
        </div>
        <div v-for="contact in contactLinks">
          <div class="d-flex flex-row info-font-size align-items-center">
            <div class="d-flex justify-content-center font-awesome-scale">
              <i class="font-awesome-rotate" :class="[contact.fontAwesomeLogo]" aria-hidden="true"
                 @mouseover="hover = true"></i>
            </div>
            <a :href="contact.text" target="_blank">{{ contact.text }}</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Bio",
  props: {
    contactInfo: Array,
    contactLinks: Array,
  }
}
</script>

<style scoped>
.headings-color {
  color: #004368;
}

.font-awesome-color {
  color: #004368;
}

.job-title-color {
  color: #b84646;
}

.info-font-size {
  font-size: 20px;
}

a {
  color: #b84646;
  text-decoration: none;
}

a:hover {
  color: #004368;
}

.font-awesome-scale:hover {
  transform: scale(1.7);
}

.font-awesome-rotate:hover {
  transform: rotate(-15deg);
}

</style>