<template>
  <div>

    <v-card class="mb-6">
      <v-img
        height="200"
        width="100%"
        src="@/assets/images/materio_img/developerMeetup.png"
      ></v-img>

      <v-card-text class="d-flex align-center mt-5 text-h4 font-weight-black">
          FIRST INSIGHTS FROM THE BEER REVIEW SITES
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



  <v-card class="mb-6">
    <v-row class="ma-0 pa-0">
      <v-col cols="8" sm="6">
        <v-card-title class="greeting-title d-flex flex-nowrap text-2xl primary--text">
          <span class="text-no-wrap font-weight-bold mx-1">From where the customers are coming from ?</span>
        </v-card-title>
      </v-col>

      <v-col cols="4" sm="6" >
        <div>
          <v-img
            width="120"
            src="@/assets/images/misc/tree-4.png"
            class="gamification-tree-4"
          ></v-img>
          <v-img
            width="121"
            src="@/assets/images/3d-characters/pose-2.png"
            class="gamification-john-pose-2"
          ></v-img>
          <v-img
            width="100"
            src="@/assets/images/misc/tree.png"
            class="gamification-tree"
          ></v-img>
        </div>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="8" sm="8" lg="8" md="8">
        <v-card>
          <v-img
          src="@/assets/images/nb_ratings_country.png"
          ></v-img>
        </v-card>
      </v-col>
      <v-col cols="4" sm="4" lg="4" md="4">
        <v-row>
          <v-card class="mb-6">
            <v-card-text>
                On this figure, we plotted the number of ratings posted in US
                in blue and the number of ratings for all the other countries in yellow.
                The y-axis is in logarithmic scale.
                <br><br>We can see that the total number of rating from the US is much higher
                than in the other countries. There are nearly
                <strong> 10 millions ratings from the US </strong>
                whereas the second country (Canada) only has 1 million.
            </v-card-text>
          </v-card>
        </v-row>
        <v-row>
          <v-card class="mb-6">
            <v-card-text>
              💡 Given the number of comments we have from the United States,
              we therefore advise our client to open his brewery in the United States.
              <br><br>Indeed, knowing that our client wants to build its
              <strong> business and market intelligence </strong>
              on the study of consumer comments, the analysis will be much more relevant in
              the United States and our client will be able to get real benefits from our work.
            </v-card-text>
          </v-card>
        </v-row>
      </v-col>
    </v-row>
  </v-card>

  <v-card class="mb-6">
    <v-row class="ma-0 pa-0">
      <v-col
        cols="8"
        sm="6"
      >
        <v-card-title class="greeting-title d-flex flex-nowrap text-2xl primary--text">
          <span class="text-no-wrap font-weight-bold mx-1">Evolution of the beer industry <br>over the past few years</span>
        </v-card-title>

      </v-col>

      <v-col
        cols="4"
        sm="6"
      >
        <div>
          <v-img
            width="121"
            src="@/assets/images/3d-characters/pose-f-28.png"
            class="gamification-john-pose-2"
          ></v-img>
          <v-img
            width="100"
            src="@/assets/images/misc/tree.png"
            class="gamification-tree"
          ></v-img>
        </div>
      </v-col>
    </v-row>
  </v-card>


  <v-card class="mb-6">
    <v-card-title>
      <span class="text-h6 primary--text font-weight-black">
        Evolution of the number of breweries involved in the ratings per year
      </span>
    </v-card-title>
    <v-card-text  class="text-subtitle-2">

      We need to understand how the current beer market behaves in US to be able to know if opening a brewery is a strategic choice for our client.
      To do this, we will determine <i>how many breweries have opened the past few years and of which kind they are</i>.

      <v-row>
        <v-avatar
            size="44"
            :color="primary"
            rounded
            class="elevation-1"
          >
            <v-icon
              dark
              color="white"
              size="30"
            >
              mdi-trending-up
            </v-icon>
          </v-avatar>

          <div class="ms-3">


          The number of breweries involved in ratings has been growing very quickly over the past decade in the United States. Indeed, we can see on Rate Beer that this evolution even follows an exponential trend since 2007. We don't need to worry about the stabilization in 2017 because the ratings we have available stop in July 2017.
          In only 10 years, the number of breweries involved in the ratings has increased
          <strong>from 1304 in 2006 to 4410 in 2016 </strong>, which corresponds to a growth of
          <strong> 238%</strong>.
          <br>Regarding Beer Advocate, there are fewer breweries involved in the ratings. We observe a peak in 2014 corresponding to about 1200 breweries, which matches the number of breweries in 2007 on Rate Beer before the explosion started.
          <br>In addition, the curve does not follow the same trend as Rate Beer and the number of breweries is decreasing since 2014.

          <br>
          Knowing that we want to study the competition on the beer market, focusing on the Rate Beer review site seems to be more relevant
          to study our client's potential competitors.
          </div>

      </v-row>
    </v-card-text>
  </v-card>
  </div>

</template>



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
