<template>
  <section>
    <h3 class="headings-color fw-bold d-flex flex-nowrap align-items-center px-lg-2"
        @click="displayingSkills"
        @mouseover="hover = true">
      <i class="fa fa-trophy pe-2 pe-md-0 pe-lg-2" aria-hidden="true"/>
      Achievements
      <i class="fa ps-2 ps-md-0 ps-lg-2"
         :class="{'fa-angle-down' : displayBlock, 'fa-angle-up' : !displayBlock}"
         aria-hidden="true"/>
    </h3>
    <div v-for="achievement in achievements"
         :class="{'d-none' : displayBlock, 'd-block' : !displayBlock}">
      <h6 class="fst-italic grey-color px-md-2">
        <i class="fa fa-certificate pe-2 headings-color" aria-hidden="true"/>
        {{ achievement }}
      </h6>
    </div>
  </section>
</template>

<script>
export default {
  name: "Achievements",
  data() {
    return {
      achievements: [
        'Award for the best student of the generation 2015/2019',
        'First place award on the national competition for the best high school company',
        'Second place award in Hackathon-“Innovative solutions in healthcare"',
        'Multiple awards in Mathematics'
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

h3:hover {
  cursor: pointer;
}
</style>