<template>
  <section id="how-to-play">
    <div class="container
      d-flex
      align-items-center
      flex-column
      mb-sm-5
      mb-lg-5
      pt-5
      pt-sm-0
      position-relative
      text-center">
      <h1 class="how-to-play font-weight-bold">HOW TO PLAY</h1>
      <h1 class="five-simple-steps font-weight-bold">5 SIMPLE STEPS</h1>
    </div>
    <StepOne></StepOne>
    <StepTwo></StepTwo>
    <StepThree></StepThree>
    <StepFour></StepFour>
    <StepFive></StepFive>
    <SuspiciousChicken></SuspiciousChicken>

  </section>
</template>
<script>
import StepOne from './StepOne.vue';
import StepTwo from './StepTwo.vue';
import StepThree from './StepThree.vue';
import StepFour from './StepFour.vue';
import StepFive from './StepFive.vue';
import SuspiciousChicken from './SuspiciousChicken.vue';


export default {
  components: {
    StepOne,
    StepTwo,
    StepThree,
    StepFour,
    StepFive,
    SuspiciousChicken,
  },
};

</script>
<style lang="scss">
@import '../assets/scss/main.scss';

.traces-container-step-four-top {}

.how-to-play {
  color: $primary;
  font-size: $h1-fsize;
}

.five-simple-steps {
  color: $secondary;
  font-size: $h1-fsize;
}

@include media-breakpoint-down(md){
  .title{
    font-size: 2.9rem;
    line-height: 2.9rem;
    font-weight: bold;
  }
}
@include media-breakpoint-down(sm){
  .title{
    font-size: 2rem;
    line-height: 2rem;
    font-weight: bold;
  }
};

</style>
