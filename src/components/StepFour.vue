<template>
  <!-- STEP 4 -->
  <div class="container fourth-step text-center position-relative">
    <div class="traces-around-container">
      <Traces count="3" rotate="60"></Traces>
      <Traces class="trace-around-block-two" count="3" rotate="70"></Traces>
      <Traces class="trace-around-block-three" count="3" rotate="25"></Traces>
      <Traces class="trace-around-block-four" count="3" rotate="5"></Traces>
      <Traces class="trace-around-block-five" count="3" rotate="-15"></Traces>
      <Traces class="trace-around-block-six" count="5" rotate="-70"></Traces>
      <Traces class="trace-around-block-seven" count="2" rotate="-10"></Traces>
    </div>
    <div class="d-flex
     flex-column
     flex-md-row
     justify-content-between
     align-items-center">
      <div class="text-center text-sm-left step font-weight-bold">4</div>
      <div class="info font-weight-bold text-center text-md-right text-uppercase">
        <p>if you complete the dare,
          draw a GOAT card and keep
          your dare card for points. </p>
      </div>
    </div>
    <div class="mobile-trace-s-four-top">
      <img src="../assets/img/mobile_trace_small.svg">
    </div>
    <div data-aos="fade-up" class="draw-dare position-relative">
      <img src="../assets/img/draw_a_goat.svg">
    </div>
    <div class="info font-weight-bold text-center text-md-right text-uppercase mx-auto mr-sm-0 ml-sm-auto">
      <p> If you don't complete the
        dare, draw a chicken card
        and take your punishment.
        Discard the dare card.</p>
    </div>
    <div class="mobile-trace-s-four-bottom"><img src="../assets/img/mobile_trace_small.svg"></div>
    <div data-aos="fade-up" class="rooster_boo-ha-re-koo text-center position-relative">
      <img src="../assets/img/rooster_boo-ha-re-koo.svg">
    </div>
    <Traces
      class="traces-container-step-four-bottom position-absolute"
      count="5"
      rotate="-10"
    ></Traces>
  </div>
  <!-- /STEP 4 -->
</template>
<script>
import Traces from './Traces.vue';

export default {
  components: {
    Traces,
  },
};

</script>
<style lang="scss">
  @import '../assets/scss/main.scss';
  .step{
    position: relative;
    z-index: 2;
  }
  .traces-container-step-four-bottom {
    right: 600px;
    bottom: -20px;
  }

  .mobile-trace-s-four-bottom,
  .mobile-trace-s-four-top {
    display: none;
  }

  .draw-dare {
    padding-top: 6.25rem;
    padding-bottom: 12rem;
  }

  .traces-around-container {
    position: absolute;
    left: 375px;
    top: -80px;
  }

  .trace-around-block-two {
    position: absolute;
    top: 95px;
    left: -215px;
  }

  .trace-around-block-three {
    position: absolute;
    top: 230px;
    left: -390px;
  }

.trace-around-block-four {
  position: absolute;
  top: 450px;
  left: -450px;
}

.trace-around-block-five {
  position: absolute;
  top: 690px;
  left: -435px;
}

.trace-around-block-six {
  position: absolute;
  top: 800px;
  left: -190px;
}

.trace-around-block-seven {
  position: absolute;
  top: 1090px;
  left: 10px;
}

.rooster_boo-ha-re-koo {
  padding-bottom: 15.625rem;
  z-index: 10;
  position: relative;
}

@include media-breakpoint-down(md) {
  .traces-around-container {
    left: 190px;
    top: -80px;
  }
  .trace-around-block-six {
    position: absolute;
    top: 545px;
    left: -190px;
  }

  .trace-around-block-seven {
    position: absolute;
    top: 820px;
    left: 20px;
  }
  .traces-container-step-four-bottom {
    right: 400px;
    bottom: -150px;
  }
  .draw-dare {
  padding-top: 8.5rem;
  padding-bottom: 4.5rem;
    img {
      max-width: 690px;
    }
  }
  .rooster_boo-ha-re-koo {
    margin-top: 3.75rem;
    padding-bottom: 0;
    margin-bottom: 8rem;
    img {
      max-width: 517px;
    }
  }
}
@include media-breakpoint-down(sm) {
  .step {
    margin-bottom: 3rem;
  }
  .mobile-trace-s-four-top {
    display: block;
    position: absolute;
    top: 200px;
    left: 50%;
    transform: translateX(-50%);
  }
  .mobile-trace-s-four-bottom {
    display: block;
    position: absolute;
    bottom: 260px;
    left: 50%;
    transform: translateX(-50%);
  }

  .draw-dare {
    padding-top: 2.5rem;
    img {
      width: 346px;
      max-width: 100%;
    }
  }
  .rooster_boo-ha-re-koo {
    margin-bottom: 5rem;
    img {
      width: 346px;
      max-width: 100%;
    }
  }
}
</style>
