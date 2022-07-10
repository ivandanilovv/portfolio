<template>
  <section>
    <h2 class="fw-bold headings-color">
      <i class="fa fa-graduation-cap" aria-hidden="true"/>
      Education
    </h2>
    <div v-for="education in educationHistory">
      <h5 class="fw-bold description-color">
        <i class="fa fa-university" aria-hidden="true"/>
        {{ education.school }}
      </h5>
      <h5 class="fst-italic grey-color">
        {{ education.title }}
      </h5>
      <h6>
        {{ education.date }}
      </h6>
    </div>
  </section>
</template>

<script>
export default {
  name: "Education",
  data() {
    return {
      educationHistory: [
        {
          school: 'Faculty of Computer Science and Engineering - Skopje',
          title: 'Computer Science',
          date: 'October, 2019 - Present'
        },
        {
          school: 'Goso Vikentiev - Kocani',
          title: 'Electrical technician for computer science and automation',
          date: 'September, 2015 - June, 2019'
        },
        {
          school: 'Ss. Cyril and Methodius- Kocani',
          title: 'Primary School',
          date: 'September, 2007 - June, 2015'
        }
      ]
    }
  }
}
</script>

<style scoped>

.grey-color {
  color: grey;
}
</style>