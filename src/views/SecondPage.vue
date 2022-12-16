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

    <v-spacer></v-spacer>

    <v-card class="mb-6" color = '#EDE7F6' height="100">
      <v-row class="ma-0 pa-0">
        <v-col cols="8" sm="6">
          <v-card-title class="greeting-title d-flex flex-nowrap text-2xl primary--text">
            <span class="text-no-wrap font-weight-bold mx-1">From where the customers are coming from ?</span>
          </v-card-title>
        </v-col>
        <v-col cols="4" sm="6" >
          <div>
            <v-img
              width="121"
              src="@/assets/images/3d-characters/pose-m-14.png"
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
      <v-container :align="center">
        <v-row>
          <v-col cols="8" sm="8" lg="8" md="8">
            <v-card>
              <v-img
                src = "@/assets/images/nb_ratings_country.png">
              </v-img>
            </v-card>
          </v-col>
          <v-col cols="4" sm="4" lg="4" md="4" :align="center" justify="space-around">
            <v-container :align="center">
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
                <v-card class="mb-4">
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
            </v-container>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-spacer></v-spacer>

    <v-card class="mb-6" color = '#EDE7F6' height="100">
      <v-row class="ma-0 pa-0">
        <v-col cols="8" sm="6">
          <v-card-title class="greeting-title d-flex flex-nowrap text-2xl primary--text">
            <span class="text-no-wrap font-weight-bold mx-1">Evolution of the beer industry over the past few years</span>
          </v-card-title>
        </v-col>

        <v-col cols="4" sm="6">
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
      <v-card class="mb-2">
        <v-card-title>
          <span class="text-xl primary--text font-weight-black">
            Evolution of the number of breweries involved in the ratings per year
          </span>
        </v-card-title>
        <v-card-text  class="text-subtitle-2">
          We need to understand how the current beer market behaves in US to be able to know if opening a brewery is a strategic choice for our client.
          To do this, we will determine <i>how many breweries have opened the past few years and of which kind they are</i>.
        </v-card-text>
      </v-card>
      <v-card class>
        <v-img
          src="@/assets/images/evolution_breweries.png">
        </v-img>
      </v-card>
      <v-card>
        <v-container :align="center">
          <v-row>
            <v-col cols='1'>
              <v-row :align="'center'">
                <v-btn class="mx-2" dark large color="primary" height='100%'>
                  <v-icon :align="center" large>
                    {{icons.mdiChartTimelineVariantShimmer}}
                  </v-icon>
                </v-btn>
              </v-row>
            </v-col>
            <v-col cols='11' :align="center">
              <v-card>
                <v-card-text>
                  The number of breweries involved in ratings has been growing very quickly over the past decade in the United States. Indeed, we can see on Rate Beer that this evolution even follows an exponential trend since 2007. We don't need to worry about the stabilization in 2017 because the ratings we have available stop in July 2017.
                  <br>In only 10 years, the number of breweries involved in the ratings has increased from
                  <strong>1304 </strong>
                  in 2006 to
                  <strong>4410</strong> in 2016 , which corresponds to a growth of
                  <strong> 238%</strong>.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
          <v-row>
            <v-card>
              <v-card-text>
                Regarding Beer Advocate, there are fewer breweries involved in the ratings. We observe a peak in 2014 corresponding to about 1200 breweries, which matches the number of breweries in 2007 on Rate Beer before the explosion started.
                <br>In addition, the curve does not follow the same trend as Rate Beer and the number of breweries is decreasing since 2014.
                <br><br>
                💡Knowing that we want to study the competition on the beer market, focusing on the Rate Beer review site seems to be more relevant
                to study our client's potential competitors.
              </v-card-text>
            </v-card>
          </v-row>
        </v-container>
      </v-card>
    </v-card>


    <v-card class="mb-6">
      <v-card class="mb-2">
        <v-card-title>
          <span class="text-xl primary--text font-weight-black">
            Evolution of the number of ratings per year
          </span>
        </v-card-title>
        <v-card-text  class="text-subtitle-2">
          The <strong>evolution of the number of breweries</strong>
          involved in the ratings might depend strongly on the
          <strong>number of ratings</strong> on the site, which could explain why the curve for Beer Advocate does not follow the same trend as the curve for Rate Beer.
          <br><br>Hence, we will study the evolution of the number of ratings for the two websites only for beers produced by American breweries.
        </v-card-text>
      </v-card>
      <v-card class>
        <v-img
          src="@/assets/images/1.png">
        </v-img>
      </v-card>
      <v-card>
        <v-card-text>
          We can indeed see that the number of ratings on Beer Advocate drops drastically from 2015, while it decreases minimally on Rate Beer (taking into account that ratings stop in July 2017).
          <br><br>Moreover, the Pearson coefficients show actually a strong linear relationship (~  0.76  for RB and ~  0.82  for BA) between the two distributions which is very significant (p-value ~  0.0002  for RB and ~  10−5  for BA).
          <br><br>This drop in the number of comments on Beer Advocate may explain why the number of breweries involved in the ratings decreases from 2015.
        </v-card-text>
      </v-card>
      <v-card class="mb-4">
        <v-card>
          <v-card-text  class="text-subtitle-2">
            Let's now compare the evolution of ratings on the two websites by plotting them on the same plot.
          </v-card-text>
        </v-card>

        <v-container>
          <v-row>
            <v-col cols="6">
              <v-card>
                <v-img
                  src="@/assets/images/2.png">
                </v-img>
              </v-card>
            </v-col>
            <v-col cols="6">
              <v-row :align="center">
                <v-card>
                  <v-card-text>
                    We can see a peak in the number of ratings between 2010 and 2016 for the two websites, with the maximum values reached in 2014.
                    <br><br>Moreover, Beer Advocate gets a higher number of ratings between 2012 and 2015 whereas Rate Beer was always above outside these dates.
                    <br><br>Hence, Beer Advocate reached a high peak in popularity in 2013/2014 with a number of ratings almost equals to 582 242 (so 6 times higher than in 2014 - 88 398 ratings), but since then, the number of ratings is higher on Rate Beer.
                  </v-card-text>
                </v-card>
              </v-row>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
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
