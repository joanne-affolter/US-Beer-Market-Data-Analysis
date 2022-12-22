<template>
    <div>
        <!--Title with image-->
        <v-card class="mb-6" color="primary">
            <v-img
                height="200"
                width="100%"
                src="@/assets/images/back.jpg"
            ></v-img>

            <v-card-text >
                    <p class = "d-flex align-center mt-5 text-h5 white--text font-weight-black">Strategic advice for market positioning in Virginia</p>
                    <p class = 'd-flex align-center mt-5 white--text'>The American beer industry has become increasingly competitive in recent years. It is therefore essential for our client to define a strategy in order to stand out from other breweries and to survive over the years.</p>
            </v-card-text>
        </v-card>

        <!-- Introduction -->
        <v-card class="mb-6 my-8">
            <v-container>
                <v-row class="ma-0 pa-0">
                  <v-col cols="12" sm="12">
                    <v-card-text class="text-subtitle-2 font-weight-bold">
                        <span class=" text-m my-6 primary--text">
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
                    <v-col cols="4" sm="4">
                        <span class="d-flex align-center mt-5 text-h6 primary--text font-weight-bold">
                            How to find similar beers ?
                        </span>
                    </v-col>
                    <v-col cols="2" sm="2">
                        <v-img
                        src="@/assets/images/question_gif.gif"
                        height="100%"
                        width="90">
                        </v-img>
                    </v-col>
                </v-row>
                </v-container>
            </v-card-title>

            <v-card-text>
                <v-container>
                    <v-row>
                        <v-col cols="5" sm="5">
                            <v-row>
                            <v-card class="mb-6" outlined border-color="primary" elevation="24">
                                <v-card-text>
                                    <div class = 'font-weight-bold'>
                                    1️⃣ Represent each beer by a vector with components :
                                    aroma, palate, appearance, taste
                                    </div>
                                    <v-card class="my-6">
                                    <v-img
                                    src="@/assets/images/rep_beer.jpg"
                                    width="300">
                                    </v-img>
                                    </v-card>
                                </v-card-text>
                            </v-card>
                            </v-row>

                            <v-row>
                                <v-card class="mb-6" outlined border-color="primary" elevation="24">
                                <v-card-text class = 'font-weight-bold'>
                                    2️⃣ Use <strong>Euclidean distance </strong> to measure similarity between beers
                                </v-card-text>
                                </v-card>
                            </v-row>
                            <v-row>
                            <v-card class="mb-6" outlined border-color="primary" elevation="24">
                                <v-card-text class = 'font-weight-bold'>
                                    3️⃣ Use <strong>k-Nearest Neighbors algorithm </strong> to get the neighbors of our client's beer which will be considered as the most similar ones
                                </v-card-text>
                            </v-card>
                            </v-row>
                        </v-col>
                        <v-col cols="7" sm="7">
                            <v-card class="mb-6" outlined border-color="primary" elevation="24">
                                <v-card-text>
                                    Let's visualize our beer vectors. But since they live in a four-dimensional space, we first need to apply a dimensionality reduction method. We have opted for
                                    <span class="primary--text">PCA</span>.
                                    <v-img
                                    src="@/assets/images/viz_beers.png">
                                    </v-img>
                                    We can see a linear dependency between the values of the two axes, with points located around the regression line with a stable variance. A sub-matching pattern seems to exist, meaning that the beers in the ratings have similarities even if we cannot interpret the values of the two axes as such.
                                </v-card-text>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-container>
            </v-card-text>
        </v-card>

        <v-card>
        <v-container>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Top 5 similar beers to our client's
              </span>
            </v-card-text>
          </v-card>
        </v-row>
        <v-row>
          <v-card>
            <v-card-text>
                Remember that our client has already gathered some reviews from his friends and family. We run our k-NN algorithm and we find the following 5 beers to be most similar to our client's.

                <v-row justify="center" align="center">
                    <v-col cols="9" sm="9">
                        <v-card class="mb-6 my-6">
                            <v-img src="@/assets/images/ratings_knn.png">
                            </v-img>
                        </v-card>
                    </v-col>
                </v-row>
                <v-row>
                    We see that our taste rating is the lowest compared to our closest competitors. On the other hand, the palate and appearance scores are relatively high. This enables us to pinpoint the problem to our client so they don't waste their resources on improving the appearance of their beer as it already rates high. Instead, he should develop other products that provide a different taste while keeping the same palate feel.
                </v-row>

            </v-card-text>
        </v-card>
        </v-row>

        <v-row>
            <Top5></Top5>
        </v-row>


        </v-container>
        </v-card>

        <!-- Influent features -->
        <v-card class="mb-6 my-6" color="primary" >
            <v-container>
                <v-row>
                    <v-col cols="12" sm="12">
                        <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                            Which features most influence the global rating?
                        </v-card-text>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>

        <v-card>
            <v-container>
                <v-row>
                    <v-card>
                        <v-card-text class='text-subtitle-2'>
                            We need to understand which features most influence the overall rating and therefore are most important to consumers to determine on which aspects our client should focus on when creating new products.
                            <br><br>Using <span class="primary--text">Linear Regression</span>, we will find out which features have the most influence on the overall rating.
                        </v-card-text>
                    </v-card>
                </v-row>

                <v-row>
                    <v-col cols="5" sm="5">
                        <v-img
                        src="@/assets/images/linreg.png">
                        </v-img>
                    </v-col>
                    <v-col cols="7" sm="7">
                        <v-card><v-card-text>
                        The taste score has the highest coefficient and thus has the biggest impact on the global rating. Appearance, on the other hand, has a coefficient that is only half as high and does not have as much influence on the consumers' score.
                        <br><br>
                        <div class='primary--text text-subtitle-2'>
                        💡 When developing new beers, our client should then focus on taste and palate, and not on appearance as he did with its existing products.
                         </div>
                        </v-card-text></v-card>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>


        <v-card class="mb-6 my-6">
            <v-card-text>
            <v-row>
                <v-col cols="7" sm="7">
                    <p class="text-subtitle-1">
                    Disappointed with the results on the potential ratings his beer could have in Virginia, our client asked us for advice on what type of beer he should produce in the state.
                    </p>
                    <v-divider></v-divider>
                    <br>
                    In response to his query, we proposed the following strategy :
                    create a flagship product that would allow him to enter the market successfully but also to last over time.
                    <br><br>
                    <p class="font-weight-bold text-h8">🤔 But how do we define this product?</p>
                    First of all, the product must attract consumers. The goal here is not to be original. Instead, we need to choose a style that is rooted in Virginia, a beer that customers will look for and want to repurchase because it is their favorite style.
                    <br><br>
                    Then, after having found the right beer style, our client must propose a product that stands out from the competitors, and therefore from the most popular beers of these styles.
                    <br><br>
                    By doing so, our client can be assured that his product will appeal to consumers, hoping that they will prefer his beer to the most popular over the state.

                </v-col>
                <v-col cols="5" sm="5">
                    <v-img
                    src="@/assets/images/sadboy.jpg"
                    >
                    </v-img>
                </v-col>
            </v-row>
            </v-card-text>
        </v-card>

        <v-card>
        <v-container>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Which style should you chose ?
              </span>
            </v-card-text>
          </v-card>
        </v-row>
        <v-row>
            <v-card class="mb-6 my-6">
            <v-img
            src="@/assets/images/styles.png"></v-img>
            </v-card>
        </v-row>

        <v-row>
            <v-card class="mb-6 my-6">
            <v-img
            src="@/assets/images/ev_styles.png"></v-img>
            </v-card>
        </v-row>

        <v-row>
            <v-card class="mb-6" outlined elevation="24">
                <v-card-text>
                Imperial IPA is the most established style in Virginia with the highest number of ratings. India Pale Ale (IPA), on the other hand, has been growing very rapidly since 2014 and is becoming more and more popular in Virginia, even surpassing Imperial IPA in the number of ratings in 2016.
                <br><br>
                Our client should therefore focus on the following styles:
                <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">
                    <v-timeline-item small color="primary">
                        <div class="d-flex justify-space-between align-center flex-wrap">
                        <h4 class="font-weight-semibold me-1">
                            <span class="primary--text">Imperial IPA</span>, a long-standing favorite in Virginia
                        </h4>
                        </div>
                    </v-timeline-item>

                    <v-timeline-item small color="primary">
                        <div class="d-flex justify-space-between align-center flex-wrap">
                        <h4 class="font-weight-semibold me-1">
                            <span class="primary--text">India Pale Ale (IPA)</span>, a style that has become increasingly popular in recent years
                        </h4>
                        </div>
                    </v-timeline-item>
                </v-timeline>
            </v-card-text>
            </v-card>
        </v-row>

        </v-container>
        </v-card>

        <v-card class="mb-6" color="#ECEFF1">
        <v-container fill-height>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                For each style, which are the most popular beers?
              </span>
            </v-card-text>
          </v-card>
        </v-row>

        <v-row>
            <v-card><v-card-text class="text-subtitle-2">
            Now that we have decided which style of beer to produce, we need to determine which beers are the most popular. This will tell us which beers we need to outperform and on which criterias we need to focus.
            </v-card-text></v-card>
        </v-row>

        <v-row>
            <v-card class="my-6">
            <v-card-title class="primary--text text-xl font-weight-bold ">
                <span class="primary--text">India Pale Ale (IPA)</span>
            </v-card-title>
            <v-row>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/red_clay.jpeg"
                    width="120" height="150"></v-img>
                    </v-card>
                    <v-card-text class="font-weight-bold">
                        Popularity : 163.17
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/ran.jpeg"
                    width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold">
                        Popularity : 87.75
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/honor.jpeg" width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold">
                        Popularity : 76.80
                </v-card-text>
            </v-col>
            </v-row>
            </v-card>
        </v-row>
        </v-container>
        </v-card>







    </div>
</template>

<script>
import TabNeighbors from '@/components/TabNeighbors.vue'
import Top5 from '@/components/Top5.vue'

export default {
  components: {
    TabNeighbors,
    Top5,
  },
  setup() {
    return {}
  },
}
</script>

