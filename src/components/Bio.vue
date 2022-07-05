<template>
  <section>
    <div class="row text-start">
      <div class="col-2 d-flex flex-column justify-content-center">
        <div class="ratio ratio-2x3">
          <img src="../assets/images/tablo_resized.jpg" alt="Profle image">
        </div>
      </div>
      <div class="col-10 col-md-3 align-bottom d-flex flex-column justify-content-center">
        <h2 class="fw-bold headingsColor">Ivan Danilov</h2>
        <h4 class="jobTitleColor">Full Stack Developer</h4>
      </div>
      <div class="col-12 col-md-5 text-start d-flex flex-column justify-content-center">
        <h3 class="fw-bold headingsColor pt-3 pt-md-0">Contact</h3>
          <p class="infoFontSize"><i class="pe-2 fa fa-phone fontAwesomeColor" aria-hidden="true"></i>+389 70296123</p>
          <p class="infoFontSize"><i class="pe-2 fa fa-envelope fontAwesomeColor" aria-hidden="true"></i>ivandanilov282@gmail.com</p>
          <p class="infoFontSize d-flex flex-nowrap"><i style="font-size:24px" class="pe-2 fa fa-linkedin-square fontAwesomeColor" aria-hidden="true"></i>http://www.linkedin.com/in/ivandanilov1</p>
          <p class="infoFontSize"><i style="font-size:25px" class="pe-3 fa fa-map-pin fontAwesomeColor" aria-hidden="true"></i>Kiril and
            Metodij 60, 2300 Kocani(Macedonia)</p>
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
.headingsColor, .fontAwesomeColor {
  color: #004368;
}

.jobTitleColor {
  color: #b84646;
}

.infoFontSize {
  font-size: 20px;
}
</style>