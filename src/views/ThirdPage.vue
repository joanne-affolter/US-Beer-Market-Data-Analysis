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
                <span class="text-h5">
                Market analysis
                </span>
                <span class="text-subtitle-2">
                    In this second part, we will determine who are the potential competitors of our client
                    and in which state he should locate its brewery.
                </span>
            </v-card-text>

        </v-card>

        <!-- Specifications -->
        <v-card>
            <v-card-title class="align-start">
                Let's note we were given the following specifications :
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
                The beer market has exploded in the United States since 2007. Americans are becoming more and more passionate about beer and breweries are opening all the time.
                <br><br>
                However, the industry has become very competitive and our client must strategically choose where to locate its brewery in a state where:
                <br><br>
                ▪️ There are beer consumers, so there is a market share to reach and potential customers
                <br>
                ▪️ There is not much competition, otherwise it will be difficult to stand out from the other breweries
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
                                As we assumed earlier, the map representing the number of breweries per state is similar to that of the number of users per state.
                                <br>Of the 10 states with the most users, 7 also have the most breweries. So there could be a lot of competition in these states. Indeed, in California and Michigan, there are only 8 customers per brewery, which does not leave much room for newcomers.
                                <br>At this stage of the analysis, we do not recommend these states to our client.
                                <br><br>
                                The states of Massachusetts and New Jersey are more interesting, since the ratio nb_users/nb_breweries is much higher.
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
                    From what we have just seen, it may be interesting to *study the ratio nb_users/nb_breweries*.              </span>
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
                Although the ratio is high in these states, some of them do not have many users (Rhode Island, Alabama) and our client may not find a suitable customer base for its products.
                <br><br>
                However, it might be interesting to study the evolution of the number of users over the last few years to determine if the demand could increase in the coming years. Our client would then gain a large market share and become a leader in states where few breweries are still established.
              </v-card-text>
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
                            We can see here that some states have seen their number of users increasing over the last few years or stabilizing, which signifies a recent and growing craze in the states. Texas, Ohio, Virginia and Idaho are the 4 states with the best evolution in the last years. The population of these states could therefore represent a potential target for our client.
                            <br><br>
                            Other states, however, have seen their number of users drop in recent years. California and Illinois are among the states with the most consumers and the most breweries. We strongly advise against these states because it seems that there was a big hype around beer in the last few years but that this fervor is decreasing.
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
                                We can see here that the percentage of ratings for local beers is increasing for most of the states. In fact, except for Alaska where the percentage is slightly decreasing since 2014, we can now confirm that Americans are turning more and more to local. We therefore strongly support our client's idea to set up a local brewery.
                                <br><br>
                                Some states are particularly catching our attention:
                                <br><br>
                                ▪️ The states of Vermont, Mississippi, Virginia, Massachusetts, Minnesota with very rapid growth since 2014
                                <br>
                                ▪️ The states of California, Colorado, Oregon, Michigan, and Ohio which are growing more slowly but are in the top 10 states with the highest percentage of local ratings in 2016 (between  40 % and  60 %).
                                <br>
                                ▪️ The remaining states may still represent potential targets for our client.
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
                                In order for our client's brewery to endure over time, we advise them to create a real community around their brewery. It would therefore be interesting to determine which states are home to consumers who are passionate about beer and who are invested in this growing community. Indeed, these are the users most likely to be interested in our client's offer.
                                <br><br>
                                We will therefore determine in which states the most active people on beer reviews sites are located.                            </v-card-text>
                        </v-card>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col>
                        <v-img src="@/assets/images/beer_lovers.png"></v-img>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col>
                        <v-card>
                            <TableLovers></TableLovers>
                        </v-card>
                    </v-col>
                    <v-col>
                        <v-card>
                            <v-card-text>
                                Idaho, leading with a very high ratio of nb_ratings/nb_users (~  77 ) and an average of 240 ratings per user has only 400 consumers. The number of ratings is lower than in other countries, but it has only 10,000 fewer ratings than Tennessee which has 4 times as many consumers. The few users that there are in this state are therefore very active in the beer community.
                                <br><br>
                                We observe the same phenomenon in Arizona and Tennessee which have a high average of ratings per user but few comments.
                                <br><br>
                                The states of Colorado, Washington and Minesota, on the other hand, have a very active community with about 93,500, 111,500 and 91,500 ratings respectively. The users seem to be very invested in the community since the average number of ratings is about 132, 125 and 126 ratings/user.
                                <br><br>
                                We therefore recommend these 3 states to our client whose beer community seems very strong. Idaho, Arizona and Tenneesse could be real potential targets with a beer loving audience.
                            </v-card-text>>
                        </v-card>
                    </v-col>
                </v-row>
            </v-container>

        </v-card>

        <v-card>
            <v-row>
                <v-col>
                    <v-img src="@/assets/images/top_states.png"></v-img>
                </v-col>
            </v-row>
        </v-card>





    </div>
</template>

<script>
import TableLovers from '@/components/TableLovers.vue'
import TableUsers from '@/components/TableUsers.vue'
import TabRatio from '@/components/TabRatio.vue'

export default {
  components: {
    TableUsers,
    TabRatio,
    TableLovers,
  },
  setup() {
    return {
      icons: {},
    }
  },
}
</script>
