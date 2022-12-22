<template>
    <div>
        <!--Title with image-->
        <v-card class="mb-6" color="primary">
            <v-img
                height="200"
                width="100%"
                src="@/assets/images/materio_img/mac-pc.png"
            ></v-img>

            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                <span class="text-h5 font-weight-black ">
                Market analysis
                </span>
            </v-card-text>

        </v-card>

        <!-- Specifications -->
        <v-card>
            <v-card-title class="align-start">
                In this second part, we will determine who are the potential competitors of our client. Let's note that our client has given us the following specifications:
                <v-spacer></v-spacer>
            </v-card-title>

            <v-card-text>
                <v-timeline dense class="timeline-custom-dense timeline-custom-dots">

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        Passionate about beer, he wants to be as close as possible to his customers and therefore wants to reach a local clientele in the state where he will set up his brewery.
                    </h4>
                    </div>
                </v-timeline-item>

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        He is not able to produce more than 30 beers.
                    </h4>
                    </div>
                </v-timeline-item>

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        He is open to all states to set up his brewery.
                    </h4>
                    </div>
                </v-timeline-item>

                </v-timeline>
                To assist our client in selecting the location for their brewery, we will first examine consumer behavior in each state. Then, we will identify competitors with a similar production capacity, meaning local breweries that produce no more than 30 beers.
            </v-card-text>
        </v-card>

        <!--I. Title with avatar-->
        <v-card class="mb-6 my-8">
            <v-container>
            <v-row class="ma-0 pa-0">
              <v-col cols="9" sm="9">
                <v-card-title class="greeting-title d-flex flex-nowrap text-2xl font-weight-bold primary--text">
                    Where should you open your brewery ?
                </v-card-title>
                <v-card-text class="text-subtitle-2 font-weight-bold">
                    In order to determine which states our client should open its brewery in, we will chose the top 3 states based on theses criterias :
                </v-card-text>
                <v-card-actions>
                    <v-container>
                        <v-row>
                            <v-btn elevation="13" rounded text x-large dark color="primary" class="my-4">
                                A large market share to reach with a lot of potential clients
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary" class="my-4">
                                Consumers who like local beers
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary" class="my-4">
                                Beer lovers who make a lot of ratings
                            </v-btn>
                        </v-row>
                    </v-container>
                </v-card-actions>
              </v-col>

              <v-col cols="3" sm="3" >
                <div>
                  <v-img
                    width="121"
                    src="@/assets/images/3d-characters/pose-2.png"
                    class="gamification-john-pose-2"
                  ></v-img>
                </div>
              </v-col>
            </v-row>
        </v-container>
        </v-card>

        <!-- 1. States with a large market share to reach -->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            States with a large market share to reach
                        </v-card-text>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>

        <!--Introduction-->
        <v-card class="mb-6">
            <v-card-text>
                The beer market in the United States has experienced significant growth in recent years, with an increasing number of breweries opening and more Americans becoming interested in beer. However, the industry has become highly competitive, and it is crucial for our client to carefully select the location for their brewery in a state where there is a market for beer and relatively little competition.
                <br>
                To begin, we will determine the locations of the users of Rate Beer and Beer Advocate.
            </v-card-text>
        </v-card>

        <!-- I.1. Users/Breweries per state -->
        <v-card class="mb-6" color="#ECEFF1">
            <v-container fill-height>
                <!-- First line -->
                <v-row align="center">

                    <!-- First column -->
                    <v-col cols="6">
                        <!-- Users per state -->
                        <v-card class="mb-6" color="#ECEFF1">
                            <v-container fill-height>
                                <v-row>
                                    <v-card width="100%" color="#9E9E9E">
                                        <v-card-text>
                                        <span class="text-subtitle-1 font-weight-medium white--text">
                                            What are the states with the most consumers ?
                                        </span>
                                        </v-card-text>
                                    </v-card>
                                </v-row>
                                <v-row>
                                    <v-col>
                                        <v-img src="@/assets/images/ratings_state.png"> </v-img>
                                    </v-col>
                                </v-row>
                            </v-container>
                        </v-card>
                    </v-col>


                    <!-- Second column -->
                    <v-col cols="6">
                        <!-- Users per state -->
                        <v-card class="mb-6" color="#ECEFF1">
                            <v-container fill-height>
                                <v-row>
                                    <v-card width="100%" color="#9E9E9E">
                                        <v-card-text>
                                        <span class="text-subtitle-1 font-weight-medium white--text">
                                            What are the states with the most breweries ?
                                        </span>
                                        </v-card-text>
                                    </v-card>
                                </v-row>
                                <v-row>
                                    <v-col>
                                        <v-img src="@/assets/images/breweries_state.png"> </v-img>
                                    </v-col>
                                </v-row>
                            </v-container>
                        </v-card>
                    </v-col>

                </v-row>

                <!-- Second line -->
                <v-row align="center">

                    <!-- First column -->
                    <v-col cols="6">
                        <!-- Recap table -->
                        <v-card class="mb-6" color="#ECEFF1">
                            <TableUsers></TableUsers>
                        </v-card>
                    </v-col>

                    <!-- Second column -->
                    <v-col cols="6">
                        <!-- Recap -->
                        <v-card class="mb-6">
                            <v-card-text>
                                We see that the number of consumers is highest in California, Pennsylvania and New York. The abundance of consumers is usually good news because it indicates a large market for our product.However, the number of breweries in these areas may also be very high, making the market saturated and the industry very competitive.
                                <br>
                                So we need to compare these results to the number of breweries installed in each state.
                                <br><br>
                                As we assumed earlier, the map representing the number of breweries per state is similar to that of the number of users per state.
                                <br>
                                Of the 10 states with the most users, 7 also have the most breweries. So there could be a lot of competition in these states. Indeed, in California and Michigan, there are only 8 customers per brewery, which does not leave much room for newcomers.
                                <br>
                                At this stage of the analysis, we do not recommend these states to our client.
                                <br><br>
                                The states of Massachusetts and New Jersey are more interesting, since the ratio nb_users/nb_breweries is higher than in the states of the previous table.
                                <br>
                                However, for Ohio, the number of breweries is very high while the number of users is not in the top 10. We therefore do not recommend this state.
                            </v-card-text>
                        </v-card>
                    </v-col>
                    </v-row>
            </v-container>
        </v-card>

        <!-- II.1. Ratio -->
        <v-card class="mb-6" color="#ECEFF1">
        <v-container fill-height>
            <v-row>
            <v-card width="100%" color="#9E9E9E">
                <v-card-text>
                <span class="text-subtitle-1 font-weight-medium white--text">
                    From what we have just seen, it may be interesting to study the ratio nb_users/nb_breweries.              </span>
                </v-card-text>
            </v-card>
            </v-row>

            <v-spacer> </v-spacer>
            <v-spacer></v-spacer>

            <v-row align="center" justify="center">
            <v-col>
                <v-card class="mb-6 mt-8">
                    <TabRatio></TabRatio>
                </v-card>
            </v-col>
            </v-row>

            <v-spacer/>

        <v-row align="center">
          <v-col>
            <v-card class="mb-6">
              <v-card-text>
                While the ratio of breweries to users is high in certain states, some of these states have a relatively small number of users (such as Rhode Island and Alabama), which may not provide a suitable customer base for our client's products. 
                <br>
                However, examining the trend in the number of users over the past few years may help us determine if demand is likely to increase in the future. This could present an opportunity for our client to establish a strong market share and become a leader in states where there are currently few established breweries.              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
        </v-card>

        <!-- 2.  Evolution of users-->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            Evolution of the number of users over the years                        </v-card-text>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card class="mb-6" color="#ECEFF1">
            <v-row>
                <v-col>
                    <v-img src="@/assets/images/ev_usersss.png"> </v-img>
                </v-col>
            </v-row>
            <v-row>
                <v-col>
                    <v-card>
                        <v-card-text>
                            We can observe that some states have seen an increase or stabilization in the number of users over the past few years, indicating a growing interest in beer in these states. Texas, Ohio, Virginia, and Idaho have particularly strong trends in recent years and may represent potential target states for our client.
                            <br>
                            On the other hand, other states have seen a decline in the number of users in recent years. California and Illinois are among the states with the highest number of consumers and breweries. We advise against these states as it appears that there was a significant interest in beer in these states in the past few years, but this enthusiasm may be diminishing.
                        </v-card-text>
                    </v-card>
                </v-col>
            </v-row>
        </v-card>

        <!-- 3. Evolution of local users -->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            Where are the local beer lovers?
                        </v-card-text>
                     </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card class="mb-6" color="#ECEFF1">
            <v-container>
                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                Our client wants to reach a local clientele in the state where he will set up his brewery, so we are going to determine which states have a preference for local products.
                                <br>
                                To do this, we will measure for each state the percentage of ratings related to beers produced in the user's state compared to the total number of ratings in the state.
                                <br>
                                Next, we will determine which states could potentially contain local beer lovers by studying the change in the percentage of local ratings over time.
                            </v-card-text>
                        </v-card>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col>
                        <v-img src="@/assets/images/ev_local.png"></v-img>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                We can see here that the percentage of ratings for local beers is increasing for most of the states. In fact, except for Alaska where the percentage is slightly decreasing since 2014, we can now confirm that Americans are turning more and more to local beers. We therefore strongly support our client's idea to set up a local brewery.
                                <br>
                                Some states are particularly catching our attention:
                                <ul>
                                    <li>The states of Vermont, Mississippi, Virginia, Massachusetts, Minnesota with very rapid growth since 2014</li>
                                    <li>The states of California, Colorado, Oregon, Michigan, and Ohio which are growing more slowly but are in the top 10 states with the highest percentage of local ratings in 2016 (between 40 % and 60 %).</li>
                                    <li>The remaining states may still represent potential targets for our client.</li>
                                </ul>
                            </v-card-text>
                        </v-card>
                    </v-col>
                </v-row>
            </v-container>

        </v-card>

        <!-- 4. Evolution of beer lovers -->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            Where are the real beer fans who make a lot of ratings ?
                        </v-card-text>
                     </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card class="mb-6" color="#ECEFF1">
            <v-container>
                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                To identify the states where the most passionate and engaged beer enthusiasts are located, we will analyze the ratio of number of ratings to number of users and the average number of ratings per user in each state using data from Rate Beer. This will allow us to determine which states have the most dedicated and active users, and therefore the most potential for building a strong community around our client's brewery. 
                                <br>
                                We will focus on Rate Beer due to its higher number of experienced users. By targeting these states, our client can establish their brewery in a location where they are likely to find an engaged and supportive customer base.
                            </v-card-text>
                        </v-card>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col cols="6">
                        <v-img src="@/assets/images/beers_lovers.png"></v-img>
                    </v-col>
                    <v-col cols="6">
                        <v-card>
                            <TableLovers></TableLovers>
                        </v-card>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                The state of Idaho has the highest ratio of number of ratings to number of users, with an average of 240 ratings per user. Although it has a lower number of ratings overall, its small number of users (400) makes it a state with very active beer consumers. 
                                <br>
                                Arizona and Tennessee also have a high average of ratings per user, but fewer total ratings. 
                                <br>
                                On the other hand, Colorado, Washington, and Minnesota have a very active beer community, with around 93,500, 111,500, and 91,500 ratings respectively and an average of around 125-132 ratings per user. We recommend that our client consider these three states, as well as Idaho, Arizona, and Tennessee, as they have a strong and invested beer community.
                            </v-card-text>
                        </v-card>
                    </v-col>
                </v-row>
            </v-container>

        </v-card>


        <!-- 5. States with the highest score
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            States with the highest score
                         </v-card-text>
                     </v-col>
                </v-row>
            </v-container>
        </v-card>
        <v-card>
            <v-row align="center" justify="center">
                <v-col cols="8">
                    <v-img src="@/assets/images/top_states.png"></v-img>
                </v-col>
            </v-row>
        </v-card>
        -->

        <!-- COMPETITORS -->
        <!--I. Title with avatar-->
        <v-card class="mb-6 my-6">
            <v-container>
            <v-row class="ma-0 pa-0">
              <v-col cols="9" sm="9">
                <v-card-title class="greeting-title d-flex flex-nowrap text-2xl font-weight-bold primary--text">
                    Which breweries are our client's competitors ?
                </v-card-title>
                <v-card-text class="text-subtitle-2 font-weight-bold">
                    <span class="my-6">
                        After investigating user behavior by state in detail, we will now complete our market research by focusing on our client's potential competitors.
                        <br>
                        We will filter the breweries according to the following criteria:
                    </span>
                    <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                We remove breweries from the states with a total score of 0. By eliminating breweries located in states with a low score, we can focus on markets that are more likely to be viable for our client's brewery. This will help to ensure that our analysis is more accurate and relevant, as it will exclude areas that may not be attractive to our client.
                            </h4>
                            </div>
                        </v-timeline-item>

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                We remove the breweries which don't have ratings in 2016/2017. We want to consider only competitors that are still in the market. Since the latest date available in the dataset is in 2017, we will remove all breweries that stopped receiving reviews prior to that date.
                            </h4>
                            </div>
                        </v-timeline-item>

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                We keep only the breweries of the same size as our client. By limiting our analysis to breweries that are the same size as our client, we can more accurately compare their capabilities and resources. This will allow us to identify potential competitors that may be more evenly matched with our client in terms of production capacity and market presence.
                            </h4>
                            </div>
                        </v-timeline-item>

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                We remove the breweries that have a very low number of ratings. Breweries with a low number of ratings may not be well-established or popular, and therefore may not pose a significant threat to our client. By removing these breweries from our analysis, we can focus on more relevant competitors that are more likely to be viable threats to our client.
                            </h4>
                            </div>
                        </v-timeline-item>

                        </v-timeline>

                        <div class="text-subtitle-2 font-weight-bold my-6">
                            Then, we will study some characteristics of the breweries to determine which ones could be our client's potential competitors, while continuing to score the states to select at the end only the best state to install our client's brewery
                            <br>
                            Note that we will focus on Rate Beer as the number of breweries is much more important than on Beer Advocate.
                        </div>
                    </v-card-text>
              </v-col>

              <v-col cols="3" sm="3" >
                <div>
                  <v-img
                    width="121"
                    src="@/assets/images/3d-characters/under-maintenance.png"
                    class="gamification-john-pose-2"
                  ></v-img>
                </div>
              </v-col>
            </v-row>
        </v-container>
        </v-card>

        <!-- Filtering - Title -->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="8" sm="6">
                        <v-card-text class="d-flex align-center mt-5 text-h6 white--text font-weight-black">
                            Number of concurrent breweries per state - After filtering
                         </v-card-text>
                     </v-col>
                </v-row>
            </v-container>
        </v-card>

        <!-- Filtering - Content -->
        <v-card class="mb-6" color="#ECEFF1">
            <v-container>
                <v-row>
                    <v-col>
                        <v-img src="@/assets/images/bilan_ranking.png"></v-img>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                <div class="text-subtitle-2 font-weight-bold my-6">
                                    The plot above shows the results of our market research. On the left you can see the number of potential competitors for our client for each state whose total score is strictly greater than 0. On the right is the ranking of the states according to the total score which corresponds to the sum of the scores obtained on the following criteria:
                                </div>
                                <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">

                                    <v-timeline-item small color="primary">
                                        <div class="d-flex justify-space-between align-center flex-wrap">
                                        <h4 class="font-weight-semibold me-1">
                                            <strong>Number of users :</strong> a high number of users and therefore a potential market to reach
                                        </h4>
                                        </div>
                                    </v-timeline-item>

                                    <v-timeline-item small color="primary">
                                        <div class="d-flex justify-space-between align-center flex-wrap">
                                        <h4 class="font-weight-semibold me-1">
                                            <strong>Number of users / Number of breweries :</strong> a low ratio and therefore a market not saturated, with less competition.
                                        </h4>
                                        </div>
                                    </v-timeline-item>

                                    <v-timeline-item small color="primary">
                                        <div class="d-flex justify-space-between align-center flex-wrap">
                                        <h4 class="font-weight-semibold me-1">
                                            <strong>Evolution of the number of users:</strong> a fast evolution since few years and a public which is getting more and more interested in beer.
                                        </h4>
                                        </div>
                                    </v-timeline-item>

                                    <v-timeline-item small color="primary">
                                        <div class="d-flex justify-space-between align-center flex-wrap">
                                        <h4 class="font-weight-semibold me-1">
                                            <strong>Evolution of the percentage of ratings on local beers :</strong> a fast evolution and consumers who are more and more attached to the local character. A potential target for our client.
                                        </h4>
                                        </div>
                                    </v-timeline-item>

                                    <v-timeline-item small color="primary">
                                        <div class="d-flex justify-space-between align-center flex-wrap">
                                        <h4 class="font-weight-semibold me-1">
                                           <strong>Average number of ratings per user :</strong> a fairly high number and therefore a strong community of beer lovers who would be interested in our client's products.
                                        </h4>
                                        </div>
                                    </v-timeline-item>

                                    </v-timeline>
                                    Based on these insights, we are now able to determine the 3 most favorable states for our client's brewery location.
                            </v-card-text>

                        </v-card>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card class="mb-6" color="primary">
            <Top3></Top3>
        </v-card>





    </div>
</template>

<script>
import TableLovers from '@/components/TableLovers.vue'
import TableUsers from '@/components/TableUsers.vue'
import TabRatio from '@/components/TabRatio.vue'
import Top3 from '@/components/Top3.vue'

export default {
  components: {
    TableUsers,
    TabRatio,
    TableLovers,
    Top3,
  },
  setup() {
    return {
      icons: {},
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
