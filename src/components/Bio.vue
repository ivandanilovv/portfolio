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
      <div class="col-12 col-md-5 text-start d-flex flex-column justify-content-center">
        <h3 class="fw-bold headings-color pt-3 pt-md-0">
          Contact
        </h3>
        <div class="d-flex flex-row info-font-size align-items-center">
          <div class="d-flex justify-content-center">
            <i class="fs-5 pe-2 fa fa-phone font-awesome-color" aria-hidden="true"></i>
          </div>
          +389 70296123
        </div>
        <div class="d-flex flex-row info-font-size align-items-center">
          <div class="d-flex justify-content-center">
            <i class="fs-5 pe-2 fa fa-envelope font-awesome-color" aria-hidden="true"></i>
          </div>
          ivandanilov282@gmail.com
        </div>
        <div class="d-flex flex-row info-font-size flex-nowrap align-items-center">
          <div class="d-flex justify-content-center">
            <i class="fs-4 pe-2 fa fa-linkedin-square font-awesome-color" aria-hidden="true"></i>
          </div>
          http://www.linkedin.com/in/ivandanilov1
        </div>
        <div class="d-flex flex-row info-font-size align-items-center">
          <div class="d-flex justify-content-center">
            <i class="fs-4 pe-3 fa fa-map-pin font-awesome-color" aria-hidden="true"></i>
          </div>
          Kiril and Metodij 60, 2300 Kocani(Macedonia)
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Bio"
}
</script>

<style scoped>
.headings-color, .font-awesome-color {
  color: #004368;
}

.job-title-color {
  color: #b84646;
}

.info-font-size {
  font-size: 20px;
}
</style>