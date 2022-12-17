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

              <v-col cols="3" sm="3" >
                <div>
                  <v-img
                    width="121"
                    src="@/assets/images/3d-characters/launching-soon.png"
                    class="gamification-john-pose-2"
                  ></v-img>
                </div>
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


    <v-card>
      <v-toolbar color="primary" dark flat>
        <v-toolbar-title>Ratings per brewery</v-toolbar-title>
        <v-spacer></v-spacer>
        <template v-slot:extension>
          <v-tabs v-model="tab" align-with-title >
            <v-tabs-slider color="yellow"></v-tabs-slider>
            <v-tab>Washington </v-tab>
            <v-tab>Virginia</v-tab>
            <v-tab>Massachusetts</v-tab>
          </v-tabs>
        </template>
      </v-toolbar>

      <v-tabs-items v-model="tab">
        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <v-img src="@/assets/images/wash1.png"></v-img>
              The 3 breweries with the highest number of comments dominate by far the other breweries in the top 10, and are the breweries to watch. Yakima Brewing and Malting Co. is far ahead of its competitors with 1,627 ratings, twice as many as the brewery just behind it.
            </v-card-text>
          </v-card>
        </v-tab-item>

          <v-tab-item>
          <v-card flat>
            <v-card-text>
              <v-img src="@/assets/images/vir1.png"></v-img>
                The distribution of the number of ratings is more uniform among the breweries here. This is not surprising, as this is the state with the most breweries in the country (33 breweries) and therefore fewer market leaders like in Washington. Howewer, we can note that Blue & Gray Brewing Co. slightly dominates the market.
            </v-card-text>
          </v-card>
        </v-tab-item>

                <v-tab-item>
          <v-card flat>
            <v-card-text>
              <v-img src="@/assets/images/m1.png"></v-img>
                The top 3 breweries here share more than half of the total number of ratings of the 10 most popular breweries, and are therefore the breweries to watch.
            </v-card-text>
          </v-card>
        </v-tab-item>

      </v-tabs-items>
    </v-card>

</div>
</template>

<script>
</script>
