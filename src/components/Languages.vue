<template>
  <section>
    <h2 class="fw-bold headingsColor"><i class="fa fa-language" aria-hidden="true"></i> Languages</h2>
    <h6 class="fst-italic greyColor">Macedonian(Native)</h6>
    <div class="progress">
      <div class="progress-bar progress-bar-striped progressBarColor" role="progressbar" style="width: 100%"
           aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">Native
      </div>
    </div>
    <h6 class="fst-italic greyColor">English</h6>
    <div class="progress">
      <div class="progress-bar progressBarColor progress-bar-striped" role="progressbar" style="width: 85%"
           aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">Fluent
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Languages"
}
</script>

<style scoped>
.progressBarColor {
  background-color: #b84646;
}

.greyColor {
  color: grey;
}

.headingsColor {
  color: #004368;
}
</style>