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
        In order to provide the most informed advice to our customers,
        we have decided to use
        <span class= 'primary--text'> Beer Advocate </span> and
        <span class= 'primary--text'> Rate Beer</span> as the primary sources for our market analysis.
        These websites are highly regarded by millions of consumers each month as the go-to resources for beer reviews and are considered to be the benchmark in the industry.
        <br><br> In order to gain a comprehensive understanding of the beer industry and consumer behavior, we will begin our analysis by exploring the data provided by these websites through initial data exploration.
      </v-card-text>
    </v-card>

    <!--I. Title with avatar-->
    <v-card class="mb-6" color="primary">
      <v-container>
        <v-row>

          <v-col cols="8" sm="8">
            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                From where the customers are coming from ?
            </v-card-text>
          </v-col>

          <v-col cols="4" sm="4">
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
            <v-img src="@/assets/images/graph.png"> </v-img>
          </v-col>

          <v-col cols="4" sm="6">
            <v-container d-flex fill-height>

              <v-row>
                <v-col>
                <v-card>
                  <v-card-text>
                    On the above figure we plotted the
                    <strong>number of ratings</strong> posted in US in blue and the number of ratings for all the other countries in yellow.
                    <br>The y-axis is in logarithmic scale.
                    <br><br>We can see that the total number of rating from the US is much higher than in the other countries.
                    There are nearly
                    <span class='primary--text'>10 millions ratings from the US </span>
                    whereas the second country (Canada) only has 1 million.                  </v-card-text>
                </v-card>
                </v-col>
              </v-row>

              <v-spacer></v-spacer>

              <v-row>
                <v-col>
                <v-card>
                  <v-card-text>
                    Based on the high volume of consumer comments from the United States, it is our recommendation that our client consider
                    <span class='primary--text'>opening its brewery in the United States</span>.
                    <br>This decision is further supported by the fact that our client wishes to use consumer comments to inform the development and growth of their business. Conducting this analysis in the United States would provide the most
                    <strong>relevant and useful insights. </strong> </v-card-text>
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

          <v-col cols="8" sm="8">
            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
              Evolution of the beer industry over the past few years
            </v-card-text>
          </v-col>

          <v-col cols="4" sm="4">
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
        In order to assess the feasibility of opening a brewery in the United States for our client, it is necessary to analyze the
        <span class='primary--text'>current state of the beer market </span>
        in the country.
        <br><br>To gather this information, we will research the number and types of breweries that have opened in the United States in recent years.
        <br> This will provide valuable insight into the market demand and competition for different types of breweries.
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
                  <span class='primary--text text-subtitle-2'>There has been significant growth in the number of breweries in the United States in recent years.</span>
                  <br><br>According to data from Rate Beer, the number of breweries has increased exponentially since 2007, going from 1304 in 2006 to 4410 in 2016, a <strong>growth of 238%</strong>.
                  <br>On the other hand, data from Beer Advocate shows a different trend, with a peak of around 1200 breweries in 2014, followed by a decrease in the number of breweries since then.
                  <br><br>
                  <span class='text-subtitle-2 font-weight-medium'>Based on these observations, it seems that studying competition in the beer market through the Rate Beer review site would be more relevant in terms of understanding potential competitors for our client.
                  </span>
                </v-card-text>
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
                It is possible that the trend in the number of breweries included in the ratings on different review sites may be influenced by the number of ratings on those sites.
                <br>This could explain the difference in trends between the data from Rate Beer and Beer Advocate.
                As such, we will investigate the
                <span class='primary--text'>evolution of the number of ratings </span>
                for American breweries on both of these websites in order to better understand these trends.
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
                Moreover, the <strong>Pearson coefficients</strong> show actually a strong linear relationship (~  0.76  for RB and ~  0.82  for BA) between the two distributions which is very significant (p-value ~  0.0002  for RB and ~  10<sup>−5</sup> for BA).
                <br><br>
                This drop in the number of comments on Beer Advocate may explain
                <i>why the number of breweries involved in the ratings decreases from 2015</i>.
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
                To gain insight into the reasons behind the spike in ratings and the shift in popularity between the two websites, we will analyze
                <span class='primary--text'>consumer behavior </span>
                on both Rate Beer and Beer Advocate.
                <br><br>
                To do this, we will divide the ratings into
                <span class='primary--text'> three periods: </span>
                <ul>
                  <li> The first period between 2007 and 2011, when Rate Beer had the most ratings. </li>
                  <li> The second period between 2012 and 2015, when Beer Advocate was the most popular. </li>
                  <li> The third period after 2015, when Rate Beer regained its leading position. </li>
                </ul>
                <br><br>
                By examining these periods separately, we can better understand the factors that influenced consumer behavior and the relative popularity of the two websites.
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
                First, it is clear that there were significantly
                <span class='primary--text'>
                more consumers on both sites between 2012 and 2015</span>:
                <ul>
                  <li><strong>107 713 </strong>users vs 32 003  before and  25 040  after for BA.</li>
                  <li><strong>61 629 </strong>users vs  24 209  before and  17 862  after for RB.</li>
                </ul>
                <br><br>This suggests that there may have been a surge of interest in trying new beers and giving opinions on review sites like Beer Advocate and Rate Beer during this period.
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
                Additionally, we see that outside of the 2012 to 2015 period, Rate Beer users tend to rate more beers on average per year than Beer Advocate users.
               <br><br>
                It is interesting to note that the average number of beers rated remains relatively constant (around 15) on Beer Advocate between 2012 and 2015, while it has decreased significantly for Rate Beer (around 16) during this period. This could be explained by the fact that many amateurs rated beers on Rate Beer during this time.            </v-card-text>
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
              <v-card-text class="text-subtitle-2">
                We can interpret these findings as follows.
                <br>Rate Beer users are more experienced and consistent in their rating activity, likely being true beer enthusiasts who are willing to try and review new beers.
                <br>On the other hand, Beer Advocate consumers seem to be more amateur in their approach, with a surge in activity between 2012 and 2015 when the number of ratings on Beer Advocate surpassed those on Rate Beer.
                <br>These consumers may have been caught up in the hype of discovering new beers during this time, but as the hype died down, their rating activity decreased.
                <br>It appears that these amateur consumers turned more to Beer Advocate, while those with more experience favored Rate Beer for their ratings.         </v-card-text>
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
                Did this hype around beers have an impact on breweries ?
              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-row align="center" justify="center">
          <v-col>
            <v-card>
              <v-card-text>
                We want to determine whether the recent growth in the number of beer ratings on review websites has had
                <span class='primary--text'>a positive impact on the brewery business
                  </span>in the United States.
                <br>To do this, we will focus on the breweries listed on Rate Beer, as there are more of them listed on this site than on Beer Advocate.
                <br><br>
                To answer the following questions, we will compare the
                <span class='primary--text'>evolution</span>
                over the years of the
                <span class='primary--text'>number of "in" breweries</span>
                (those that appear for the first time in the ratings) and
                <span class='primary--text'>"out" breweries </span>
                (those that no longer appear in the ratings).
                <br><br>
                <div class="text-subtitle-2">
                <ul>
                  <li>Were the breweries already known to users on the beer review sites or did new breweries appear in the ratings? </li>
                  <li>Do users easily adopt a new brewery and continue rating it over time after their first rating?</li>
                </ul>
                </div>
                <br><br>
                By examining these trends, we can better understand the success and sustainability of new breweries in the market.
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
          <v-col cols="7">
            <v-card color="#C8E6C9">
              <v-card-title>
                'In' breweries
              </v-card-title>
              <v-card-text>
                While the number of 'in' breweries remained relatively low between 2004 and 2008, it then saw a rapid increase until reaching 841 new breweries in the ratings in 2016.
                <br><br>This growth appears to be closely connected to the increase in interest and activity in the beer market in the United States starting in 2012, as there were approximately 150 new 'in' breweries added each year between 2011 and 2014, corresponding to the spike in ratings we observed earlier.
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="5">
            <v-card color="#FFCDD2">
              <v-card-title>
                'Out' breweries
              </v-card-title>
              <v-card-text>
                The number of 'out' breweries, or those that are no longer included in the ratings, remained relatively stable until 2012 and then saw a sharp increase to 730 'out' breweries in 2016, almost the same number as the 'in' breweries that year.
                <br><br>
                This could potentially be linked to the increased competition in the market and the presence of hundreds of new breweries each year.
                <br><br>
                <div class="text-subtitle-2">
                To better understand the nature of these 'out' breweries, we will separate them based on the number of years between their first and last rating.
                </div>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <v-row>
          <v-col>
            <v-card>
              <v-card-text>
                💡 Further analysis would be needed to determine the direction of causality between the two trends : whether the influx of new breweries drove the desire among Americans to discover new beers, or if the trend of discovering new beers prompted an increase in the number of new breweries.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
    </v-container>
    </v-card>

    <!-- II.4. Impact on breweries 2 -->
    <v-card class="mb-6" color="#ECEFF1">
      <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                But what are these 'out' breweries? Are they old breweries that have been surpassed by the new 'in' breweries?
                Or do the new breweries appearing in the comments fail to last?
              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-row align="center">
          <v-col class="mb-6 mt-4">
            <Table></Table>
          </v-col>
        </v-row>

        <v-spacer/>

        <v-row align="center">
          <v-col>
            <v-card class="mt-4">
              <v-card-text>
                <div class="text-subtitle-2">
                In the table above, we have grouped the breweries according to the difference between the year of the first and last rating. We also calculated the average number of comments per beer for each category, and the average rate.
                </div>
                <br><br>
                We can see here that  6  % of the breweries disappear in the ratings the same year as the first rating. Moreover, the average number of ratings per beer is almost equal to  1.
                <br>
                <span class='primary--text'>
                These breweries have not been able to break through the competition.
                </span>
                <br><br>
                We have observed that the percentage of breweries decreases as the number of years between their first and last rating increases, while the average number of ratings per beer increases.
                <span class='primary--text'>
                This suggests that new breweries that appear in the ratings tend to not last over time and may struggle to maintain consumer interest.
                </span>
                <br><br>
                However, those breweries that have been successful in establishing themselves in the industry tend to see an increase in the average number of comments over time. It is worth noting that the percentage of breweries with more than 5 years between their first and last comment is relatively small, around 16.5%.
            </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <!-- Conclusion -->
    <v-card class="mb-6" color="primary">
      <v-container>
        <v-row>

          <v-col cols="8" sm="6">
            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                Conclusion
            </v-card-text>
          </v-col>

          <v-col cols="4" sm="6">
            <v-img
              width="121"
              src="@/assets/images/3d-characters/pose-m-34.png"
              class="gamification-john-pose-2"
            ></v-img>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-card class="mb-6">
      <v-card-text>
        <v-timeline dense class="timeline-custom-dense timeline-custom-dots">

        <v-timeline-item small color="primary">
          <div class="d-flex justify-space-between align-center flex-wrap">
            <h4 class="font-weight-semibold me-1">
              Our analysis highlighted a rapid growth in the number of breweries included in the ratings, which rose from 1,304 in 2006 to 4,410 in 2016, representing a 238% increase. This growth was accompanied by a surge in the number of ratings on Rate Beer and Beer Advocate, likely due to an influx of amateur beer enthusiasts.
            </h4>
          </div>
        </v-timeline-item>
        <v-timeline-item small color="primary">
          <div class="d-flex justify-space-between align-center flex-wrap">
            <h4 class="font-weight-semibold me-1">
              The highly competitive nature of the industry is reflected in the fact that many new breweries struggle to maintain consumer interest over time, with more than half of the new breweries on the market receiving comments on their beers for only one year.
              <br>
              <span class='primary--text'>
              Our client will need to be particularly mindful of this challenge and focus on ways to differentiate their brewery and retain customers.
              </span>
            </h4>
          </div>
        </v-timeline-item>
        <v-timeline-item small color="primary">
          <div class="d-flex justify-space-between align-center flex-wrap">
            <h4 class="font-weight-semibold me-1">
              To help our client maximize their chances of success, we will conduct a competitive analysis to determine the most strategic location for their brewery and identify opportunities to outperform the competition. We will focus on Rate Beer for this analysis, as it has a larger number of breweries included in the ratings.
            </h4>
          </div>
        </v-timeline-item>
        <v-timeline-item small color="primary">
          <div class="d-flex justify-space-between align-center flex-wrap">
            <h4 class="font-weight-semibold me-1">
              Additionally, we will use Rate Beer to analyze the characteristics of a beer that appeal to a more experienced and discerning audience, such as the associations of flavors, aromas, and palates, in order to provide the most informed advice on recipe selection.
            </h4>
          </div>
        </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-card>

</div>

</template>

<script>
import Period from '@/components/Period.vue'
import Period2 from '@/components/Period2.vue'
import Table from '@/components/Table.vue'

import { mdiChartTimelineVariantShimmer, mdiLightbulbQuestionOutline, mdiMeteor } from '@mdi/js'

export default {
  components: {
    Period,
    Period2,
    Table,
  },
  setup() {
    return {
      icons: {
        mdiChartTimelineVariantShimmer,
        mdiMeteor,
        mdiLightbulbQuestionOutline,
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
