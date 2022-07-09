<template>
  <section>
    <h2 class="fw-bold headings-color pb-1"
        @click="displayingSkills"
        @mouseover="hover = true">
      <i class="fa fa-laptop" aria-hidden="true"/>
      Skills
      <i id="angleSkills" class="fa"
         :class="{'fa-angle-down' : displayBlock, 'fa-angle-up' : !displayBlock}"
         aria-hidden="true"/>
    </h2>
    <div id="skills" :class="{'d-none' : displayBlock, 'd-block' : !displayBlock}">
      <div class="row">
        <div v-for="skill in skills" class="col-6 col-md-12">
          <h6 class="fst-italic grey-color">
            {{ skill }}
          </h6>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      skills: [
        'HTML5',
        'CSS3',
        'Bootstrap',
        'Javascript',
        'Vue.js',
        'C++',
        'Git',
        'Java',
        'SQL and relational databases',
      ],
      displayBlock: true,
    }
  },
  methods: {
    displayingSkills() {
      this.displayBlock = !this.displayBlock;
    }
  }
}
</script>

<style scoped>

.grey-color {
  color: grey;
}

h2:hover {
  cursor: pointer;
}
</style>