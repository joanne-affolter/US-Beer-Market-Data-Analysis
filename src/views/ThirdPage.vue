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
        <v-row>
        <v-col cols="12" md="7" lg="7">
          <v-card>
            <v-row class="ma-0 pa-0">
              <v-col
                cols="8"
                sm="6"
              >
                <v-card-title class="greeting-title d-flex flex-nowrap text-2xl">
                    Where should you open your brewery ?
                </v-card-title>
              </v-col>

              <v-col
                cols="4"
                sm="6"
              >
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
          </v-card>
        </v-col>
    </v-row>

        <!-- Introduction -->
        <v-card class="mb-6">
                <v-card-text>
                    In order to determine which states our client should open its brewery in, we will chose the top 3 states based on thses criterias :
                </v-card-text>
                <v-actions>
                    <v-row >

                        <v-col>
                            <v-btn elevation="13" rounded text x-large dark color="primary">
                                A large market share to reach with a lot of potential clients
                            </v-btn>
                        </v-col>

                    </v-row>
                    <v-row align='center' justify="center">
                        <v-col>
                            <v-btn elevation="13" rounded text x-large dark color="primary">
                                Consumers who like local beers
                            </v-btn>
                        </v-col>

                        <v-col>
                            <v-btn elevation="13" rounded text x-large dark color="primary">
                                Beer lovers who make a lot of ratings
                            </v-btn>
                        </v-col>
                    </v-row>
                </v-actions>
        </v-card>

        <!-- 1. States with a large market share to reach -->
        <v-card class="mb-6" color="primary">
        <v-container>
            <v-row>
            <v-col cols="8" sm="6">
                <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                    States with a large market share to reach
               </v-card-text>
            </v-col>
            </v-row>
        </v-container>
        </v-card>





    </div>
</template>

<script>
</script>
