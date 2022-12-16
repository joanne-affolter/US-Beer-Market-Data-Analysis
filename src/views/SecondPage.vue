<template>
  <div>
    <!--Title with image-->
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

    <!--Introduction-->
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

    <!--I. Title with avatar-->
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

    <!-- I.1. Subpart-->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                First, we will count the number of ratings per country in order to see from where the customers are coming from.
              </span>
            </v-card-text>
          </v-card>

        </v-row>

        <v-row>

          <v-col cols="8" sm="6">
            <v-img src="@/assets/images/nb_ratings_country.png"> </v-img>
          </v-col>

          <v-col cols="4" sm="6">
            <v-container d-flex fill-height>

              <v-row>
                <v-col>
                <v-card>
                  <v-card-text>
                    On the above figure we plotted the number of ratings posted in US in blue and the number of ratings for all the other countries in yellow. The y-axis is in logarithmic scale.
                    We can see that the total number of rating from the US is much higher than in the other countries. There are nearly 10 millions ratings from the US whereas the second country (Canada) only has 1 million.
                  </v-card-text>
                </v-card>
                </v-col>
              </v-row>

              <v-spacer></v-spacer>

              <v-row>
                <v-col>
                <v-card>
                  <v-card-text>
                    Given the number of comments we have from the United States, we therefore advise our client to open his brewery in the United States.
                    Indeed, knowing that our client wants to build its business and market intelligence on the study of consumer comments, the analysis will be much more relevant in the United States and our client will be able to get real benefits from our work.
                  </v-card-text>
                </v-card>
                </v-col>
              </v-row>
            </v-container>
          </v-col>

        </v-row>

      </v-container>
    </v-card>

    <!--II. Title with avatar-->
    <v-card class="mb-6" color="primary">
      <v-container>
        <v-row>

          <v-col cols="8" sm="6">
            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
              Evolution of the beer industry over the past few years            </v-card-text>
          </v-col>

          <v-col cols="4" sm="6">
            <v-img
              width="121"
              src="@/assets/images/3d-characters/pose-f-28.png"
              class="gamification-john-pose-2"
            ></v-img>
          </v-col>

        </v-row>
      </v-container>
    </v-card>

    <!-- Introduction -->
    <v-card class="mb-6">
      <v-card-text>
        We need to understand how the current beer market behaves in US to be able to know if opening a brewery is a strategic choice for our client.
      </v-card-text>
    </v-card>

    <!-- II.1. Number of breweries -->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                How many breweries have opened the past few years ?
              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-spacer> </v-spacer>
        <v-spacer></v-spacer>

        <v-row align="center" justify="center">
          <v-col>
            <div class="my-8">
              <v-img src="@/assets/images/evolution_breweries.png"> </v-img>
            </div>
          </v-col>
        </v-row>

        <v-spacer/>

        <v-row align="center">
          <v-col>
            <v-card>
              <v-card-text>
                <v-icon large color="primary">{{icons.mdiChartTimelineVariantShimmer}}</v-icon>

                  The number of breweries involved in ratings has been growing very quickly over the past decade in the United States. Indeed, we can see on Rate Beer that this evolution even follows an exponential trend since 2007. We don't need to worry about the stabilization in 2017 because the ratings we have available stop in July 2017.
                  In only 10 years, the number of breweries involved in the ratings has increased from  1304  in 2006 to  4410  in 2016, which corresponds to a growth of  238%

                  <br><br>

                  Regarding Beer Advocate, there are fewer breweries involved in the ratings. We observe a peak in 2014 corresponding to about 1200 breweries, which matches the number of breweries in 2007 on Rate Beer before the explosion started. In addition, the curve does not follow the same trend as Rate Beer and the number of breweries is decreasing since 2014.

              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row align="center">
          <v-col>
            <v-card>
              <v-card-text>
                Knowing that we want to study the competition on the beer market, focusing on the Rate Beer review site seems to be more relevant to study our client's potential competitors.              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <!-- II.2. Number of ratings -->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Evolution of the number of ratings per year
              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-spacer></v-spacer>
        <v-spacer></v-spacer>


        <v-row align="center">
          <v-col>
            <v-card class="mb-6 my-8">
              <v-card-text class="text-subtitle-2 font-weight-medium">
                The evolution of the number of breweries involved in the ratings might depend strongly on the number of ratings on the site, which could explain why the curve for Beer Advocate does not follow the same trend as the curve for Rate Beer.
                <br><br>
                Hence, we will study the evolution of the number of ratings for the two websites only for beers produced by American breweries.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row align="center">
          <v-col>
            <div>
              <v-img src="@/assets/images/1.png"> </v-img>
            </div>
          </v-col>
        </v-row>

        <v-spacer/>

        <v-row align="center">
          <v-col>
            <v-card class="mt-8">
              <v-card-text>
                We can indeed see that the number of ratings on Beer Advocate drops drastically from 2015, while it decreases minimally on Rate Beer (taking into account that ratings stop in July 2017).
                <br><br>
                Moreover, the Pearson coefficients show actually a strong linear relationship (~  0.76  for RB and ~  0.82  for BA) between the two distributions which is very significant (p-value ~  0.0002  for RB and ~  10−5  for BA).
                <br><br>
                This drop in the number of comments on Beer Advocate may explain why the number of breweries involved in the ratings decreases from 2015.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row align="center">
          <v-col cols="6" md="6">
            <div class="my-8">
              <v-img src="@/assets/images/2.png"> </v-img>
            </div>
          </v-col>

          <v-col cols="6" md="6">
            <v-card>
              <v-card-text>
                We can see a peak in the number of ratings between 2010 and 2016 for the two websites, with the maximum values reached in 2014.

                <br><br>Moreover, Beer Advocate gets a higher number of ratings between 2012 and 2015 whereas Rate Beer was always above outside these dates.

                <br><br>Hence, Beer Advocate reached a high peak in popularity in 2013/2014 with a number of ratings almost equals to 582 242 (so 6 times higher than in 2014 - 88 398 ratings), but since then, the number of ratings is higher on Rate Beer.
              </v-card-text>
            </v-card>

          </v-col>
        </v-row>

      </v-container>
    </v-card>

    <!-- II.3. Number of users -->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Evolution of consumers behavior              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-row align="center" justify="center">
          <v-col>
            <v-card>
              <v-card-text>
                Let's check how consumers behave on both websites to understand why we get this spike in ratings and why Beer Advocate got a higher number of ratings between 2012 and 2015.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-spacer> </v-spacer>
        <v-spacer></v-spacer>

        <v-row align="center" justify="center">
          <v-col cols="8">
            <Period></Period>
          </v-col>

          <v-col cols="4">
            <v-card>
              <v-card-text>
                First, the number of consumers is significantly higher between 2012 and 2015 on both sites.
                It is therefore possible that there was a big hype in the United States during between 2012 and 2015 and that many *new consumers *started to test new beers and to give their opinions on sites such as Beer Advocate and Rate Beer.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row align="center">
          <v-col cols="8">
            <Period2></Period2>
          </v-col>

          <v-col cols="4">
            <v-card>
              <v-card-text>
                Secondly, we can see that outside of the 2012 to 2015 period, Rate Beer users rate on average many more beers than Beer Advocate users.
                <br>Note that the average number of beers rated remains stable (around 15) on BA between 2012 and 2015, whereas it has dropped significantly for RB (around 16).
                <br>That could be explained by the fact that many amateurs gave ratings on RB during that period.               </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-spacer/>

        <v-row align="center">
          <v-col>
            <v-card class="mt-6">
              <v-card-title>
                ✏️ Conclusion
              </v-card-title>
              <v-card-text>
                Rate Beer users are therefore a more confirmed public, which has not changed much over the years. They must be real passionate by beers and do not hesitate to test new ones and give their opinion.

                <br><br>Beer Advocate consumers, on the other hand, correspond more to a public of amateurs, who became passionate about beer during a few years (from 2012 to 2015), when the number of ratings exploded on Beer Advocate and overtook Rate Beer.

                <br><br>Our interpretation, then, would be that many people got into this fad of discovering new beers during this period, but that hype died down pretty quickly and users started rating fewer and fewer beers.

                <br><br>These consumers caught up in that hype turned more to Beer Advocate, while those with more experience favor Rate Beer for their ratings.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

      </v-container>
    </v-card>

    <!-- II.4. Impact on breweries -->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Do this hype around beers in US had an impact on breweries ?              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-row align="center" justify="center">
          <v-col>
            <v-card>
              <v-card-text>
                <v-list>
                  <v-list-item class="pa-0">
                    <v-icon large color="primary">{{icons.mdiMeteor}}</v-icon>
                    The number of breweries involved in the reviews has grown very quickly. <i>Were these breweries already known to users on the beer review sites or did new breweries appear in the ratings ?</i>
                  </v-list-item>
                  <v-list-item class="pa-0">
                    <v-icon large color="primary">{{icons.mdiMeteor}}</v-icon>
                    <i>Do users adopt easily a new brewery and continue to keep rating it over time after the first rating?</i>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-spacer> </v-spacer>
        <v-spacer></v-spacer>

        <v-row align="center">
          <v-col>
            <div>
              <v-img src="@/assets/images/3.png"> </v-img>
            </div>
          </v-col>
        </v-row>

      <v-row align="center">
          <v-col cols="8">
            <v-card color="#C8E6C9">
              <v-card-title>
                'In' breweries
              </v-card-title>
              <v-card-text>
                While the number of 'in' breweries remain quite low between 2004 and 2008, it then explodes until it reaches  841  new breweries in the ratings in 2016.
                <br>The quick growth in the number of 'in' breweries seems to be strongly related to the hype in the US around beer and the increase in the number of comments starting in 2012. From 2011 to 2014, there are approximately  150  new 'in' breweries each year, which matched well with the spike in the number of ratings we observed earlier.
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="4">
            <v-card color="#FFCDD2">
              <v-card-title>
                'Out breweries'
              </v-card-title>
              <v-card-text>
                The number of 'out' breweries remains stable until 2012 and then increases very sharply to 730 'out' breweries in 2016, which is almost the same number as the 'in' breweries that year! which also seems to be related to the hype around beer in the US, and the strong competition in this field where hundreds of breweries appear every year.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row>
          <v-col>
            <v-card>
              <v-card-text>
                <v-icon large color="primary">{{icons.mdiLightbulbQuestion}}</v-icon>
                We would have to take the analysis further to determine where the causal link is: Did the number of new breweries generate this desire among Americans to discover new beers? Or are people taking advantage of this trend to open breweries?
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

      <v-spacer/>
    </v-container>
  </v-card>


</div>

</template>

<script>
import Period from '@/components/Period.vue'
import Period2 from '@/components/Period2.vue'

import { mdiChartTimelineVariantShimmer, mdiLightbulbQuestion, mdiMeteor } from '@mdi/js'

export default {
  components: {
    Period,
    Period2,
  },
  setup() {
    return {
      icons: {
        mdiChartTimelineVariantShimmer,
        mdiMeteor,
        mdiLightbulbQuestion,
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
