<template>
  <div>
  <v-card class="mb-6" color="primary">
    <v-card-title>
      <p class="text-h4 white--text font-weight-black">
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

  <v-card class="mb-6" color="#B388FF">
    <v-card-title>
      <p class="text-h5 white--text font-weight-black">
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
          <v-row>
            <v-card class="mb-6">
              <v-card-text>
                On this figure, we plotted the number of ratings posted in US
                in blue and the number of ratings for all the other countries in yellow.
                The y-axis is in logarithmic scale.
                <br>We can see that the total number of rating from the US is much higher
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
              Indeed, knowing that our client wants to build its
              <strong> business and market intelligence </strong>
              on the study of consumer comments, the analysis will be much more relevant in
              the United States and our client will be able to get real benefits from our work.
              </v-card-text>
            </v-card>
          </v-row>
        </v-col>
      </v-row>
    </v-card-text>
  </v-card>

  <v-card class="mb-6" color="#B388FF">
    <v-card-title>
      <p class="text-h5 white--text font-weight-black">
        Evolution of the beer industry over the past few years
      </p>
    </v-card-title>
  </v-card>

  <v-card class="mb-6">
    <v-card-title>
      <p class="text-h6 primary--text font-weight-black">
        Evolution of the number of breweries involved in the ratings per year
      </p>
    </v-card-title>
    <v-card-text  class="primary--text text-subtitle-2">
      We need to understand how the current beer market behaves in US to be able to know if opening a brewery is a strategic choice for our client.
      To do this, we will determine <i>how many breweries have opened the past few years and of which kind they are</i>.
    </v-card-text>
  </v-card>


  <v-card class="mb-6">

    <v-card-text>
      <v-card>
        <v-img
          src="@/assets/images/evolution_breweries.png"
        ></v-img>
      </v-card>

      <v-icon
      >📈</v-icon>
      The number of breweries involved in ratings has been growing very quickly over the past decade in the United States. Indeed, we can see on Rate Beer that this evolution even follows an exponential trend since 2007. We don't need to worry about the stabilization in 2017 because the ratings we have available stop in July 2017.
      In only 10 years, the number of breweries involved in the ratings has increased
      <strong>from 1304 in 2006 to 4410 in 2016 </strong>, which corresponds to a growth of
      <strong> 238%</strong>.
      Regarding Beer Advocate, there are fewer breweries involved in the ratings. We observe a peak in 2014 corresponding to about 1200 breweries, which matches the number of breweries in 2007 on Rate Beer before the explosion started. In addition, the curve does not follow the same trend as Rate Beer and the number of breweries is decreasing since 2014.

      <br>
      Knowing that we want to study the competition on the beer market, focusing on the Rate Beer review site seems to be more relevant
      to study our client's potential competitors.

    </v-card-text>
  </v-card>


  <v-card class="mb-6">
    <v-card-title>
      <p class="text-h6 primary--text font-weight-black">
        Evolution of the number of ratings per year
      </p>
    </v-card-title>
  </v-card>

  <v-card class="mb-6">
    <v-card-text>
      The evolution of the number of breweries involved in the ratings might depend strongly on the number of ratings on the site, which could explain why the curve for Beer Advocate does not follow the same trend as the curve for Rate Beer.

Hence, we will study the evolution of the number of ratings for the two websites only for beers produced by American breweries.
      </v-card-text>
  </v-card>

  <v-card class="mb-6">
    <v-card-title>
      <p class="text-h6 primary--text font-weight-black">
        Evolution of consumers behavior
      </p>
    </v-card-title>
  </v-card>

  <v-card class="mb-6">
    <v-card-title>
      <p class="text-h6 primary--text font-weight-black">
        Evolution of consumers behavior
      </p>
    </v-card-title>
  </v-card>

  <v-card class="mb-6">
    <v-card-title>
      <p class="text-h6 primary--text font-weight-black">
        Do this hype around beers in US had an impact on breweries ?      </p>
    </v-card-title>
  </v-card>

  </div>

</template>
