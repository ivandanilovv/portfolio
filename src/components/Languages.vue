<template>
  <section>
    <h2 class="ps-lg-2 fw-bold headings-color"><i class="fa fa-language" aria-hidden="true"></i>
      Languages
    </h2>
    <h6 class="fst-italic grey-color">
      Macedonian(Native)
    </h6>
    <div class="progress">
      <div class="progress-bar progress-bar-striped progress-bar-color" role="progressbar" style="width: 100%"
           aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">Native
      </div>
    </div>
    <h6 class="fst-italic grey-color">
      English
    </h6>
    <div class="progress">
      <div class="progress-bar progress-bar-color progress-bar-striped" role="progressbar" style="width: 85%"
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
.progress-bar-color {
  background-color: #b84646;
}

.grey-color {
  color: grey;
}

.headings-color {
  color: #004368;
}
</style>