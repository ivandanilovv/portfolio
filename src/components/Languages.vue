<template>
  <section>
    <h2 class="ps-lg-2 fw-bold headings-color"><i class="fa fa-language" aria-hidden="true"></i>
      Languages
    </h2>
    <div v-for="language in progressBarLanguages">
      <h6 class="fst-italic grey-color">
        {{ language.languageName }}
      </h6>
      <div class="progress">
        <div class="progress-bar progress-bar-striped progress-bar-color" role="progressbar"
             :style="{width: language.progressBarWidth}" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">
          {{ language.progressBarDescription }}
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Languages",
  data() {
    return {
      progressBarLanguages: [
        {
          languageName: 'Macedonian(Native)',
          progressBarWidth: '100%',
          progressBarDescription: 'Native'
        },
        {
          languageName: 'English',
          progressBarWidth: '85%',
          progressBarDescription: 'Fluent'
        }
      ]
    }
  }
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