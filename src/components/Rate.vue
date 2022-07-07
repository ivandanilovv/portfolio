<template>
  <section>
    <h3 class="fw-bold headings-color px-2"><i class="fa fa-star" aria-hidden="true"></i>
      Rate my portfolio
    </h3>
    <h5 class="descriptionColor text-center">Leave a rating from 1 to 5</h5>
    <div class="px-2 text-center">
      <p class="fs-4">
        <button class="btn fs-4" @click="decreaseRating"><i class="fa fa-minus-square headings-color"
                                                            aria-hidden="true"></i></button>
        {{ rating }}
        <button class="btn fs-4" @click="increaseRating"><i class="fa fa-plus-square headings-color"
                                                            aria-hidden="true"></i></button>
        <br/>
        <button class="btn btn-info fs-5" @click="submitRating">Submit</button>
      </p>
      <div class="averageRatingMessageFontSize descriptionColor" v-if="averageRating>0">Average rating is:
        <span v-if="!isNaN(averageRating)">{{ averageRating.toFixed(2) }}
          <span v-for="index in Math.floor(averageRating)">
            <i class="fa fa-star" aria-hidden="true"></i>
          </span>
          <span v-if="averageRating*100%100>0">
            <i class="fa fa-star-half-o" aria-hidden="true"></i>
          </span>
          <span v-for="index in 5-Math.ceil(averageRating)">
            <i class="fa fa-star-o" aria-hidden="true"></i>
          </span>
        </span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Rate",
  data() {
    return {
      rating: 1,
      numberOfReviews: 0,
      sumOfReviews: 0
    }
  },
  methods: {
    increaseRating() {
      if (this.rating + 1 > 5) {
        alert("Rating can't be greater than 5!")
      } else
        this.rating++;
    },
    decreaseRating() {
      if (this.rating - 1 < 1) {
        alert("Rating can't be less than 1!")
      } else
        this.rating--;
    },
    submitRating() {
      this.sumOfReviews += this.rating;
      this.numberOfReviews++;
      this.rating = 1;
      alert("Thank you for your review!");
    }
  },
  computed: {
    averageRating() {
      return this.sumOfReviews / this.numberOfReviews;
    }
  }
}
</script>

<style scoped>
.headings-color {
  color: #004368;
}

.descriptionColor {
  color: #b84646;
}
.averageRatingMessageFontSize{
  font-size: 1.17rem;
}
</style>