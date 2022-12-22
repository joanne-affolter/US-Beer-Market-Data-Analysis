<template>
    <div>
        <!--Title with image-->
        <v-card class="mb-6" color="primary">
            <v-img
                height="200"
                width="100%"
                src="@/assets/images/beer_page5.jpg"
            ></v-img>

            <v-card-text >
                    <p class = "d-flex align-center mt-5 text-h5 white--text font-weight-black">Strategic advice for market positioning in Virginia</p>
                    <p class = 'd-flex align-center mt-5 text-subtitle-1 white--text font-weight-black'>The American beer industry has become increasingly competitive in recent years. It is therefore essential for our client to define a strategy in order to stand out from other breweries and to survive over the years.</p>
            </v-card-text>
        </v-card>

        <!-- Introduction -->
        <v-card class="mb-6 my-8">
            <v-container>
                <v-row class="ma-0 pa-0">
                  <v-col cols="12" sm="12">
                    <v-card-text class="text-subtitle-2 font-weight-bold">
                        <span class=" text-m my-6">
                            In this section, we will study the market in Virginia in detail to give our client advice on how to position itself as a market leader.                        </span>

                        <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">

                            <v-timeline-item small color="primary">
                                <div class="d-flex justify-space-between align-center flex-wrap">
                                <h4 class="font-weight-semibold me-1">
                                    First, we'll see if our client's products can reach consumers in Virginia. First, we will determine which similar beers can be found on the market and see if they are liked by consumers in Virginia.                                </h4>
                                </div>
                            </v-timeline-item>

                            <v-timeline-item small color="primary">
                                <div class="d-flex justify-space-between align-center flex-wrap">
                                <h4 class="font-weight-semibold me-1">
                                    Then, we will advise our client on the production of its new products to help him establish its position in the market and outperform its competitors.                                </h4>
                                </div>
                            </v-timeline-item>
                            </v-timeline>
                        </v-card-text>
                  </v-col>
                </v-row>
            </v-container>
        </v-card>

        <!-- More similar beers -->
        <v-card class="mb-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="12" sm="12">
                        <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                            Which beers are most similar to our products?                        </v-card-text>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card class="mb-6">
            <v-card-title>
                <v-container>
                <v-row align="center">
                    <v-col cols="2" sm="2">
                        <v-img src="@/assets/images/question_gif.gif">
                        </v-img>
                    </v-col>
                    <v-col cols="10" sm="10">
                        <span class="text-m my-6 primary--text">
                            How to find similar beers ?
                        </span>
                    </v-col>
                </v-row>
                </v-container>
            </v-card-title>

            <v-card-text>
                <v-container>
                    <v-row>
                        <v-col cols="6" sm="6">
                            <v-card class="mb-6">
                                <v-card-text>
                                    1️⃣ Represent each beer by a vector with components :
                                    <div class="font-weight-bold primary--text">
                                    <br> ▪️ aroma
                                    <br> ▪️ palate
                                    <br> ▪️ appearance
                                    <br> ▪️ taste
                                    </div>
                                    <v-img src="@/assets/images/rep_beer.jpg">

                                    </v-img>
                                </v-card-text>
                            </v-card>
                        </v-col>
                        <v-col cols="6" sm="6">
                            <v-row>
                            <v-card class="mb-6" color="primary">
                                <v-card-text>
                                    2️⃣ Use Euclidean distance to measure similarity between beers
                                </v-card-text>
                            </v-card>
                            </v-row>
                            <v-row>
                            <v-card class="mb-6" color="primary">
                                <v-card-text>
                                    3️⃣ Use Euclidean distance to measure similarity between beers
                                </v-card-text>
                            </v-card>
                            </v-row>
                        </v-col>
                    </v-row>
                </v-container>
            </v-card-text>
        </v-card>
    </div>
</template>
