<template>
  <section>
    <h2 class="fw-bold headings-color"><i class="fa fa-laptop" aria-hidden="true"></i>
      Skills
    </h2>
    <div v-for="skill in skills">
      <h6 class="fst-italic grey-color">{{ skill }}</h6>
    </div>
  </section>
</template>

<script>
export default {
  name: "Skills",
  data(){
    return{
      skills: ['HTML5', 'CSS3', 'Bootstrap', 'Javascript', 'Vue.js', 'SQL and relational databases', 'C++', 'Git', 'Java']
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
</style>