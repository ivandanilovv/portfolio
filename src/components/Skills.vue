<template>
  <section>
    <h2 class="fw-bold headings-color"><i class="fa fa-laptop" aria-hidden="true"></i>
      Skills <i id="angleSkills" class="fa" :class="{'fa-angle-down' : displayBlock, 'fa-angle-up' : !displayBlock}"
                aria-hidden="true"
                @click="displayingSkills" @mouseover="hover = true"></i>
    </h2>
    <div id="skills" :class="{'d-none' : displayBlock, 'd-block' : !displayBlock}">
      <div v-for="skill in skills">
        <h6 class="fst-italic grey-color">{{ skill }}</h6>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      skills: ['HTML5', 'CSS3', 'Bootstrap', 'Javascript', 'Vue.js', 'SQL and relational databases', 'C++', 'Git', 'Java'],
      counter: 1,
      fontAwesomeSign: 'fa fa-angle-down',
      displayBlock: true,
    }
  },
  methods: {
    displayingSkills() {
      this.displayBlock = !this.displayBlock;
      this.counter++;
    }
  }
}
</script>

<style scoped>
.headings-color {
  color: #004368;
}

.grey-color {
  color: grey;
}

#angleSkills:hover{
  cursor: pointer;
}
</style>