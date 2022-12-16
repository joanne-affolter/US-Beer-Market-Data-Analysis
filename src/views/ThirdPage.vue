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
              <v-col cols="8" sm="8">
                <v-card-title class="greeting-title d-flex flex-nowrap text-2xl font-weight-bold primary--text">
                    Where should you open your brewery ?
                </v-card-title>
                <v-card-text class="text-subtitle-2 font-weight-bold">
                    In order to determine which states our client should open its brewery in, we will chose the top 3 states based on theses criterias :
                </v-card-text>
                <v-card-actions>
                    <v-container>
                        <v-row>
                            <v-btn elevation="13" rounded text x-large dark color="primary">
                                A large market share to reach with a lot of potential clients
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary">
                                Consumers who like local beers
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary">
                                Beer lovers who make a lot of ratings
                            </v-btn>
                        </v-row>
                    </v-container>
                </v-card-actions>
              </v-col>

              <v-col cols="4" sm="4" >
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

        <!-- I.1. Users per state -->
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




    </div>
</template>

<script>
import TableUsers from '@/components/TableUsers.vue'
export default {
  components: {
    TableUsers,
  },
  setup() {
    return {
      icons: {},
    }
  },
}
</script>
