<template>
  <main class="container py-5">
    <section>
      <div class="row text-start ">
        <div class="col-2 d-flex flex-column justify-content-center">
          <div class="ratio ratio-2x3">
            <img src="../assets/images/tablo_resized.jpg" alt="Profle image">
          </div>
        </div>
        <div class="col-3 align-bottom d-flex flex-column justify-content-center">
          <h2 style="font-weight: bold; color: #004368">Ivan Danilov</h2>
          <h4>Full Stack Developer</h4>
        </div>
        <div class="col text-start d-flex flex-column justify-content-center">
          <h3 style="color: #004368; font-weight: bold">Contact</h3>
          <h5><i class="fa fa-phone" aria-hidden="true"></i> (+389) 70296123 </h5>
          <h5><i class="fa fa-envelope" aria-hidden="true"></i> ivandanilov282@gmail.com</h5>
          <h5><i class="fa fa-linkedin-square" aria-hidden="true"></i> http://www.linkedin.com/in/ivandanilov1</h5>
          <h5><i class="fa fa-map-pin" aria-hidden="true"></i> Kiril and Metodij 60, 2300 Kocani(Macedonia)</h5>
        </div>
      </div>
    </section>

    <section class="container pt-5">
      <div class="row">
        <div class="col-9 text-start">
          <div id="aboutMe">
            <h2 style="font-weight: bold; color: #004368">About me</h2>
            <h5>I am student at 3rd year at the Faculty of Computer Science and Engineering and I am highly motivated to
              learn new technologies and to become extraordinary full stack
              developer.</h5>
          </div>
          <div id="education" class="pt-3">
            <h2 style="font-weight: bold; color: #004368"><i class="fa fa-graduation-cap" aria-hidden="true"></i>Education
            </h2>
            <h5 style="color: #b84646; font-weight: bold"><i class="fa fa-university" aria-hidden="true"></i>Goso
              Vikentiev - Kocani</h5>
            <h5 style="font-style: italic; color: grey">Electrical technician for computer science and automation</h5>
            <h6>September, 2015 - June, 2019</h6>
            <h5 style="color: #b84646; font-weight: bold" class="pt-4"><i class="fa fa-university"
                                                                          aria-hidden="true"></i>Faculty of Computer
              Science and Engineering - Skopje</h5>
            <h5 style="font-style: italic; color: grey">Computer Science</h5>
            <h6>October, 2019 - Present</h6>
          </div>
        </div>
        <div class="col text-start">
          <h2 style="font-weight: bold; color: #004368">Skills</h2>
          <h6 style="font-style: italic; color: grey">HTML5</h6>
          <h6 style="font-style: italic; color: grey">CSS3</h6>
          <h6 style="font-style: italic; color: grey">Bootstrap</h6>
          <h6 style="font-style: italic; color: grey">Javascript</h6>
          <h6 style="font-style: italic; color: grey">Vue.js</h6>
          <h6 style="font-style: italic; color: grey">SQL and relational databases</h6>
          <h6 style="font-style: italic; color: grey">C++</h6>
          <h6 style="font-style: italic; color: grey">Git</h6>
          <h6 style="font-style: italic; color: grey">Java</h6>
          <h2 style="font-weight: bold; color: #004368">Languages</h2>
          <h6 style="font-style: italic; color: grey">Macedonian(Native)</h6>
          <div class="progress">
            <div class="progress-bar progress-bar-striped progressBarColor" role="progressbar" style="width: 100%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">Native</div>
          </div>
          <h6 style="font-style: italic; color: grey">English</h6>
          <div class="progress">
            <div class="progress-bar progressBarColor progress-bar-striped" role="progressbar" style="width: 85%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">Fluent</div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  components: {}
}
</script>
<style scoped>
  .progressBarColor{
    background-color: #b84646;
  }
</style>
