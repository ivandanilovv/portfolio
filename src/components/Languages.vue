<template>
  <section>
    <h2 class="ps-lg-2 pt-2 fw-bold headings-color d-flex flex-nowrap align-items-center"
        @click="displayingLanguages"
        @mouseover="hover = true">
      <i class="fa fa-language pe-2" aria-hidden="true"/>
      Languages<i id="angle" class="fa ps-2 ps-md-0 ps-lg-2"
                  :class="{'fa-angle-down' : displayBlock, 'fa-angle-up' : !displayBlock}"
                  aria-hidden="true"/>
    </h2>
    <div id="languages" :class="{'d-none' : displayBlock, 'd-block' : !displayBlock}">
      <div v-for="language in progressBarLanguages">
        <h6 class="fst-italic grey-color">
          {{ language.languageName }}
        </h6>
        <div class="progress">
          <div class="progress-bar progress-bar-color" role="progressbar"
               :style="{width: language.progressBarWidth}"
               aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">
            {{ language.progressBarDescription }}
          </div>
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
          languageName: 'Macedonian',
          progressBarWidth: '100%',
          progressBarDescription: 'Native'
        },
        {
          languageName: 'English',
          progressBarWidth: '85%',
          progressBarDescription: 'Fluent'
        }
      ],
      displayBlock: true,
    }
  },
  methods: {
    displayingLanguages() {
      this.displayBlock = !this.displayBlock
    }
  },
  computed: {},
  watch: {}
}
</script>

<style scoped>
.progress-bar-color {
  background: linear-gradient(45deg, #e3a39e, #b84646);
}

.grey-color {
  color: grey;
}

h2:hover {
  cursor: pointer;
}
</style>