<template>
  <div>
  <v-card class="mb-6" color="primary">
    <v-card-title>
      <p class="text-h3 white--text font-weight-black">
        First insights from the beer reviews
        <br>websites
      </p>
    </v-card-title>
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

  <v-card class="mb-6" color="purple lighten-5">
    <v-card-title>
      <p class="text-h4 primary--text font-weight-black">
        From where the customers are coming from ?
      </p>
    </v-card-title>
  </v-card>

  <v-card>
    <v-card-text>
      <v-row>
        <v-col cols="8" sm="8" lg="8" md="8">
          <v-card>
            <v-img

              src="@/assets/images/nb_ratings_country.png"
            ></v-img>
          </v-card>
        </v-col>
        <v-col cols="4" sm="4" lg="4" md="4">
          <v-card>
            <v-card-text>
              On the above figure we plotted the number of ratings posted in US
              in blue and the number of ratings for all the other countries in yellow.
              The y-axis is in logarithmic scale.
              <br>We can see that the total number of rating from the US is much higher
              than in the other countries. There are nearly 10 millions ratings from the US whereas the second country (Canada) only has 1 million.
            </v-card-text>
        </v-card>
        </v-col>
      </v-row>
    </v-card-text>
  </v-card>

  <v-row>

    <v-card>

    </v-card>
  </v-row>


  </div>

</template>
