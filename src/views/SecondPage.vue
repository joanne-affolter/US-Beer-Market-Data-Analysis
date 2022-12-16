<template>
  <div>

    <v-card class="mb-6" color="primary">
      <v-img
        height="200"
        width="100%"
        src="@/assets/images/materio_img/developerMeetup.png"
      ></v-img>

      <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
          Fist insights from the beer review sites
      </v-card-text>
    </v-card>

    <v-card class="mb-6">
      <v-card-text>
          We have chosen to base our market analysis on two beer review sites:
          <span class= 'primary--text'> Beer Advocate </span> and
          <span class= 'primary--text'> Rate Beer</span>.
              These two sites are widely considered the go-to beer resource for
          millions of consumers each month and the benchmark for beer reviews.
          <br> Indeed, in order to understand the demand of our customers and to adapt
          our offer as well as possible, <i>isn't it worth getting information directly from them ?</i>
          <br>
          We start our work with a first data exploratory of the two websites to understand the evolution
          of the beer industry over the last years as well as the behavior of beer consumers.
      </v-card-text>
    </v-card>

    <v-card class="mb-6" color="primary">
      <v-container>
        <v-row>

          <v-col cols="8" sm="6">
            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                From where the customers are coming from ?
            </v-card-text>
          </v-col>

          <v-col cols="4" sm="6">
            <v-img
              width="121"
              src="@/assets/images/3d-characters/pose-m-14.png"
              class="gamification-john-pose-2"
            ></v-img>
          </v-col>

        </v-row>
      </v-container>
    </v-card>


</div>

</template>

<script>
import { mdiChartTimelineVariantShimmer } from '@mdi/js'

export default {
  setup() {
    return {
      icons: {
        mdiChartTimelineVariantShimmer,
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.gamification-tree-4,
.gamification-john-pose-2,
.gamification-tree {
  position: absolute;
}
.gamification-tree {
  top: 10%;
  right: 0;
}
.gamification-john-pose-2 {
  bottom: 0;
  right: 15%;
}
.gamification-tree-4 {
  bottom: 0;
  right: 30%;
}

@media (max-width: 600px) {
  .gamification-tree,
  .gamification-tree-4 {
    display: none;
  }
  .gamification-john-pose-2 {
    right: 5%;
  }
}

@media (max-width: 500px) {
  .gamification-john-pose-2 {
    max-width: 70px;
  }
}

@media (max-width: 400px) {
  .greeting-title {
    font-size: 1.2rem !important;
  }
}

// rtl
.v-application {
  &.v-application--is-rtl {
    .gamification-john-pose-2 {
      right: initial;
      left: 15%;
    }
    .gamification-tree {
      right: initial;
      left: 0;
    }
    .gamification-tree-4 {
      left: 30%;
      right: initial;
    }
  }
}
</style>
