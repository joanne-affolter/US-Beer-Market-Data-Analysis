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
                    <span class=" text-m my-6">
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
                    height="80%"
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
                <v-col cols="12" sm="12">
                    <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                            Which breweries are the most popular in each state ?
                    </v-card-text>
                </v-col>
            </v-row>
        </v-container>
    </v-card>


    <v-card>
        <v-card-title>Ratings per brewery</v-card-title>
          <v-tabs color="primary">

            <v-tab>Washington </v-tab>
            <v-tab>Virginia</v-tab>
            <v-tab>Massachusetts</v-tab>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="10" sm="10"><v-img src="@/assets/images/wash1.png"></v-img></v-col></v-row>
                    <v-row>
                The 3 breweries with the highest number of comments dominate by far the other breweries in the top 10, and are the breweries to watch. Yakima Brewing and Malting Co. is far ahead of its competitors with 1,627 ratings, twice as many as the brewery just behind it.
                </v-row></v-container>
            </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="10" sm="10"><v-img src="@/assets/images/vir1.png"></v-img></v-col></v-row>
                    <v-row>
                    The distribution of the number of ratings is more uniform among the breweries here. This is not surprising, as this is the state with the most breweries in the country (33 breweries) and therefore fewer market leaders like in Washington. Howewer, we can note that Blue & Gray Brewing Co. slightly dominates the market.
                    </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                <v-container><v-row align="center" justify="center">
                    <v-col cols="7"><v-img src="@/assets/images/m1.png"></v-img></v-col></v-row>
                <v-row>
                    The top 3 breweries here share more than half of the total number of ratings of the 10 most popular breweries, and are therefore the breweries to watch.
                </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>
        </v-tabs>
    </v-card>

    <v-card class="mb-6 my-6">
        <v-card-text class="font-weight-black">
            We can observe that there are generally fewer ratings per brewery in Virginia: the most popular brewery has only 346 ratings, while this number is much higher in Massachusetts (1627) and Virginia (1493). This means that there are fewer popular breweries dominating the market. The sector will be less competitive for our client, which is a positive point.
        </v-card-text>
    </v-card>

    <!-- Number of years -->
    <v-card class="mb-6" color="primary" >
        <v-container>
            <v-row>
                <v-col cols="12" sm="12">
                    <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                        Which breweries are well-established in the market ?
                    </v-card-text>
                </v-col>
            </v-row>
        </v-container>
    </v-card>

    <v-card>
        <v-card-title>Number of years since first rating</v-card-title>
          <v-tabs color="primary">

            <v-tab>Washington </v-tab>
            <v-tab>Virginia</v-tab>
            <v-tab>Massachusetts</v-tab>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="10" sm="10"><v-img src="@/assets/images/w2.png"></v-img></v-col></v-row>
                    <v-row>
                        The 10 oldest breweries in the comments have been in the area for a long time: 17 years for the first one, 16 for the second one, and 14 for the next 3. These breweries can be real competitors and might be institutions in Washington. Furthermore, given the large number of established breweries in the area, Washington users may not instinctively go to new breweries and turn to the state's established breweries by habit.                </v-row></v-container>
            </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="8" sm="8"><v-img src="@/assets/images/v2.png"></v-img></v-col></v-row>
                    <v-row>
                        The difference between long-established breweries in the comments and newer breweries is much more pronounced in Virginia than in Washington. Williamsburg Brewing Company, in the lead, has been appearing in the comments for 16 years, followed closely by Founders Restaurant & Brewing Co. (14 years) and Blue & Gray Brewing Co. (13 years).

                        <br><br>He get much lower results for the other breweries. The 10th brewery, for example, got its first rating only 3 years ago.

                        <br><br>Most of the breweries in Virginia are therefore very new whereas it is the state with the largest number of potential competitors (33 breweries). Of these 33 breweries, only 5 have been in the comments for more than 7 years. Thus, our client will be able to find its place in the market more easily than in Washington, knowing that it has also the highest score regarding the evolution of the number of users for several years.                    </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                <v-container><v-row align="center" justify="center">
                    <v-col cols="7" sm="7"><v-img src="@/assets/images/m2.png"></v-img></v-col></v-row>
                <v-row>
                    In Massachusetts, 4 breweries are present in the comments since 15 years and dominate the other breweries in the top 10. Except for Gardner Ale House, the period since the first rating is twice as long as in the other breweries.

                    <br><br>We find the same pattern as in Virginia, with only 5 breweries appearing in the comments for more than 10 years. These are the ones to watch, but the market is quite favorable for our client.                </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>
        </v-tabs>
    </v-card>

    <v-card class="mb-6 my-8">
        <v-card-text class="font-weight-black">
            There are a large number of long-established breweries in Washington. We do not recommend this state because the competition could be tough. The number of institutions is lower in Virginia and Massachusetts, which seems to be more suitable for our client.        </v-card-text>
    </v-card>


    <!-- Number of locals -->
    <v-card class="mb-6" color="primary" >
        <v-container>
            <v-row>
                <v-col cols="10" sm="8">
                    <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                        Which are the local breweries ?
                    </v-card-text>
                </v-col>
            </v-row>
        </v-container>
    </v-card>

    <v-card>
        <v-card-title>Percentage of local ratings</v-card-title>
          <v-tabs color="primary">

            <v-tab>Washington </v-tab>
            <v-tab>Virginia</v-tab>
            <v-tab>Massachusetts</v-tab>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="8" sm="8"><v-img src="@/assets/images/w3.png"></v-img></v-col></v-row>
                    <v-row>
                        The percentage of local ratings is very high for these 10 breweries, ranging from 62% for Ghostfish Brewing Company to almost 95% for Top Rung Brewing Company. This suggests an audience in Washington with a preference for local beers, which is very interesting for our client.
                    </v-row>
                    </v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                    <v-container><v-row align="center" justify="center">
                        <v-col cols="8" sm="8"><v-img src="@/assets/images/v3.png"></v-img></v-col></v-row>
                    <v-row>
                        The percentage of local ratings is much lower in Virginia than in Washington. In fact, only 61% of the ratings are local for the first brewery, which is 1% less than the last brewery in the top 10 of Washington.
                        <br><br>However, the population in Virginia seems to be more and more interested in local beers as it has the highest score for the evolution of the percentage of local ratings. Our client could therefore position itself as a market leader with its brewery.
                      </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>

            <v-tab-item>
            <v-card flat>
                <v-card-text>
                <v-container><v-row align="center" justify="center">
                    <v-col cols="8" sm="8"><v-img src="@/assets/images/m3.png"></v-img></v-col></v-row>
                <v-row>
                    Similarly to Virginia, the trend for local is less pronounced than in Washington. Moreover, the percentage of local ratings is quite tight for the breweries in the top 10. Down the Road Beer Company still stands out among the other breweries.
                </v-row></v-container>
                </v-card-text>
            </v-card>
            </v-tab-item>
        </v-tabs>
    </v-card>

    <v-card class="mb-6 my-8">
        <v-card-text class="font-weight-black">
            Washington stands out from the other two states with a very high percentage of local ratings for the 10 breweries in the top 10. Even though these breweries are potential competitors, there is a very strong trend for local here and that is why we recommend this state.
        </v-card-text>
    </v-card>


    <!-- Results -->
    <v-card class="mb-6" color="primary">
        <v-img
            height="200"
            width="100%"
            src="@/assets/images/res_img.jpg"
        ></v-img>

        <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
            Results
        </v-card-text>
    </v-card>


    <v-card>
        <v-img src="@/assets/images/virginia.gif">


        </v-img>
    </v-card>











</div>
</template>

<script>
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
