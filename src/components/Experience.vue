<template>
  <section>
    <h2 class="fw-bold headings-color">
      <i class="fa fa-certificate" aria-hidden="true"/>
      Experience
    </h2>
    <div v-for="exp in experience">
      <h5 class="fw-bold description-color">
        <i class="fa fa-university" aria-hidden="true"/>
        {{ exp.companyName }}
      </h5>
      <h5 class="fst-italic grey-color">
        {{ exp.jobTitle }}
      </h5>
      <h6>{{ exp.date }}</h6>
    </div>
  </section>
</template>

<script>
export default {
  name: "Experience",
  data () {
    return {
      experience: [
        {
          companyName: 'Bike Computer Co.',
          jobTitle: 'Full Stack Developer',
          date: 'July, 2022 - Present'
        }
      ]
    }
  }
}
</script>

<style scoped>
.grey-color{
  color: grey;
}
</style>