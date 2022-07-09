<template>
  <section>
    <h3 class="px-2 ps-sm-0 ps-md-2 fw-bold headings-color d-flex flex-nowrap align-items-center">
      <i class="fa fa-star pe-2" aria-hidden="true"/>
      Rate my portfolio
    </h3>
    <h5 class="description-color text-center">
      Leave a rating from 1 to 5
    </h5>
    <div class="px-2 text-center">
      <p class="fs-4">
        <button class="btn fs-4" @click="decreaseRating">
          <i class="fa fa-minus-square headings-color" aria-hidden="true"/>
        </button>
        <span class="fs-2 fw-bold description-color">{{ rating }}</span>
        <button class="btn fs-4" @click="increaseRating">
          <i class="fa fa-plus-square headings-color" aria-hidden="true"/>
        </button>
        <br/>
        <button class="btn btn-info fs-5" @click="submitRating">
          Submit
        </button>
      </p>
      <!-- The average rating will be shown only when there is at least 1 rating submitted -->
      <div class="average-rating-message-font-size description-color" v-if="averageRating>0">
        Average rating is:
        <span v-if="!isNaN(averageRating)">{{ averageRating.toFixed(2) }}
          <!-- Number of full stars shown -->
          <span v-for="index in Math.floor(averageRating)">
            <i class="fa fa-star" aria-hidden="true"/>
          </span>
          <span v-if="averageRating*100%100>0">
            <i class="fa fa-star-half-o" aria-hidden="true"/>
          </span>
          <!-- Number of empty stars shown -->
          <span v-for="index in 5-Math.ceil(averageRating)">
            <i class="fa fa-star-o" aria-hidden="true"/>
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
      sumOfReviews: 0,
      numberOfReviews: 0,
    }
  },
  methods: {
    increaseRating() {
      if (this.rating + 1 > 5)
        alert("Rating can't be greater than 5!")
      else
        this.rating++;
    },
    decreaseRating() {
      if (this.rating - 1 < 1)
        alert("Rating can't be less than 1!")
      else
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
.average-rating-message-font-size{
  font-size: 1.17rem;
}
</style>