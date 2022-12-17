<template>
<div>
    <!--Title with image-->
    <v-card class="mb-6" color="primary">
        <v-img
            height="200"
            width="100%"
            src="@/assets/images/front4.jpg"
        ></v-img>

        <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                Leading breweries in the 3 recommended states
        </v-card-text>
    </v-card>

    <!-- Introduction -->
    <v-card class="mb-6 my-8">
        <v-container>
            <v-row class="ma-0 pa-0">
              <v-col cols="9" sm="9">
                <v-card-text class="text-subtitle-2 font-weight-bold">
                    <span class="my-6">
                        To detect potential competitors of our client, we will find which breweries...
                    </span>
                    <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                Are the most popular with the highest number of ratings
                            </h4>
                            </div>
                        </v-timeline-item>

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                Have been established in the area for a long time with the longest period since the first rating
                            </h4>
                            </div>
                        </v-timeline-item>

                        <v-timeline-item small color="primary">
                            <div class="d-flex justify-space-between align-center flex-wrap">
                            <h4 class="font-weight-semibold me-1">
                                Are local with the highest percentage of ratings within the state
                            </h4>
                            </div>
                        </v-timeline-item>

                        </v-timeline>

                        <div class="text-subtitle-2 font-weight-bold my-6">
                            By examining these criteria, we will assign scores to each brewery and then determine which ones are the strongest on the market and therefore represent the biggest competitors of our client.
                            <br><br>In parallel, we will compare the 3 states to finally retain one for the next part of our work.
                        </div>
                    </v-card-text>
              </v-col>
            </v-row>
        </v-container>
        </v-card>

    <!-- Number of ratings -->
    <v-card class="mb-6" color="primary" >
        <v-container>
            <v-row>
                <v-col cols="8" sm="6">
                    <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                        <span class="text-h5 font-weight-black ">
                        Highest number of ratings
                        </span>
                        <span class="text-subtitle-2">
                            We'll start by determining which breweries are the most popular in each state looking at the total number of ratings per brewery.
                        </span>
                    </v-card-text>
                </v-col>
            </v-row>
        </v-container>
    </v-card>


</div>
</template>

<script>
</script>
