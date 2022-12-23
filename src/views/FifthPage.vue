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
                                    First, we'll see if our client's products can reach consumers in Virginia. We will then determine which similar beers can be found on the market and see if they are liked by consumers in Virginia.                                </h4>
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
                                    <br><br>
                                    The 2-dimensional PCA representation of the data appears to show a linear dependency between the values of the two axes, with points distributed around a regression line with a consistent variance.
                                    <br>
                                    It appears that there may be sub-matching patterns present in the data, indicating that the beers in the ratings have similarities even though we cannot interpret the exact meanings of the values on the two axes.
                                    <br><br>
                                    Overall, this suggests that the original data has a strong, predictable relationship between the variables and may be amenable to linear modeling techniques.                                </v-card-text>
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
                    We see that our taste rating is the lowest compared to our closest competitors. On the other hand, the palate and appearance scores are relatively high. This enables us to pinpoint the problem to our client so he doesn't waste its resources on improving the appearance of its beers as it already rates high. Instead, he should develop other products that provide a different taste while keeping the same palate feel.
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
                            In order to understand
                            <span class='primary--text'>which features are most important to consumers </span>
                            and have the greatest influence on the overall rating of a product, we will use
                            <span class='primary--text'>
                            linear regression
                            </span>
                            to identify the relative importance of each feature.
                            <br><br>
                            By analyzing the coefficients of the linear regression model, we can determine
                            <span class='primary--text'>
                            which features have the most impact on the predicted outcome
                            </span>
                            and are therefore considered the most important.
                            <br><br>
                            This information can be used to guide the development of new products by focusing on the aspects that are most important to consumers.
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
                    In response to our client's request, we proposed the following strategy :
                    create a flagship product that would allow him to enter the market successfully but also to last over time.
                    <br><br>
                    <p class="font-weight-bold text-h8">🤔 But how do we define this product?</p>
                    To define the flagship product, it is important to focus on creating a product that will attract and retain consumers.
                    <br>
                    This means choosing a style of beer that is popular and well-liked by customers in Virginia, rather than trying to be too original or experimental.
                    <br>By selecting a style that is already rooted in the local market, our client's beer will have a higher chance of success because customers will be more familiar with and likely to seek out this type of beer.
                    <br><br>
                    Additionally, by producing a beer that customers enjoy and want to repurchase, our client can build a loyal customer base and establish a lasting presence in the market.

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

        <v-card class="mb-6" color="#ECEFF1">
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
            <br><br>Note that we defined the following score to find beers we are interested in :
            <span class="primary--text">popularity = number_of_ratings x average_rating  </span>
            </v-card-text></v-card>
        </v-row>

        <v-row>
            <v-col cols="6" sm="6">
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
                    <v-card-text class="font-weight-bold my-2">
                        Score : 163.17
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/ran.jpeg"
                    width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold my-2">
                        Score : 87.75
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/honor.jpeg" width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold my-2">
                        Score : 76.80
                </v-card-text>
            </v-col>
            </v-row>
            </v-card>
            </v-col>
            <v-col cols="6" sm="6">
            <v-card class="my-6">
            <v-card-title class="primary--text text-xl font-weight-bold ">
                <span class="primary--text">Imperial IPA</span>
            </v-card-title>
            <v-row>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/stone2.png"
                    width="120" height="150"></v-img>
                    </v-card>
                    <v-card-text class="font-weight-bold my-2">
                        Score : 292.4
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/apoca.jpeg"
                    width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold my-2">
                        Score : 164.5
                    </v-card-text>
            </v-col>
            <v-col cols="4" sm="4">
                <v-card>
                    <v-img
                    src="@/assets/images/stone3.jpg" width="120" height="150"></v-img>
                </v-card>
                <v-card-text class="font-weight-bold my-2">
                        Score : 111
                </v-card-text>
            </v-col>
            </v-row>
            </v-card>
            </v-col>
        </v-row>

        <v-row>

        </v-row>
        </v-container>
        </v-card>

        <v-card class="mb-6" color="#ECEFF1">
        <v-container>
        <v-row>
          <v-card width="100%" color="#9E9E9E">
            <v-card-text>
              <span class="text-subtitle-1 font-weight-medium white--text">
                Which characteristics make the top beers stand out?
              </span>
            </v-card-text>
          </v-card>
        </v-row>
        <v-row>
            <v-card width="100%" >
            <v-card-text class="text-subtitle-2 font-weight-bold">
                <span class = 'font-weight-lite'>
                In this section, we will analyze the most popular beers to determine which features have the greatest influence on their ratings.                 <span class=" text-m my-6 primary--text">
                </span>
                <br><br>
                By understanding which characteristics are most important to consumers, we can identify :                </span>
                <v-timeline dense class="timeline-custom-dense timeline-custom-dots mt-6">

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        Areas to focus on in order to maximize the rating of our client's beer and potentially surpass the competition
                    </h4>
                    </div>
                </v-timeline-item>

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        Specific features that can be improved or emphasized in order to enhance the overall appeal and appeal of the beer                    </h4>
                    </div>
                </v-timeline-item>
                </v-timeline>
                </v-card-text>
            </v-card>
        </v-row>
        <v-row>
            <v-card class="mb-6 my-6">
                <v-card-title class="text--primary font-weight-bold">
                    <span class="text--primary">India Pale Ale (IPA)</span>
                </v-card-title>
                <v-card-text>
                    <v-row>
                        <v-col cols="12" sm="12">
                        <v-card class="mb-6 my-6">
                        <v-img src="@/assets/images/f1.png"></v-img>
                        </v-card>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col cols="8" sm="8">
                            <v-card class="mb-6 my-6">
                            <v-img src="@/assets/images/f2.png"></v-img>
                            </v-card>
                        </v-col>
                        <v-col cols="4" sm="4">
                            <v-card class="mb-6 my-6">
                                Based on the plot, it appears that
                                <span class="primary--text">
                                taste is the most influential factor
                                </span>
                                on overall ratings for the popular beers of the regular IPA style.
                                <br><br>
                                The three leading beers stand out from their competitors due to their high ratings in this category, rather than their appearance or palate, which our client may have thought were more important factors.
                                <br><br>
                                This suggests that taste is a particularly important consideration for consumers when evaluating and rating beers, and that
                                <span class="text-subtitle-2">
                                focusing on producing a beer with a highly rated taste may be crucial for success in the market.
                                </span>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-card-text>
            </v-card>
        </v-row>

        <v-row>
            <v-card class="mb-6 my-6">
                <v-card-title class="text--primary font-weight-bold">
                    <span class="text--primary">Imperial IPA</span>
                </v-card-title>
                <v-card-text>
                    <v-row>
                        <v-col cols="12" sm="12">
                        <v-card class="mb-6 my-6">
                        <v-img src="@/assets/images/f3.png"></v-img>
                        </v-card>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col cols="8" sm="8">
                            <v-card class="mb-6 my-6">
                            <v-img src="@/assets/images/f4.png"></v-img>
                            </v-card>
                        </v-col>
                        <v-col cols="4" sm="4">
                            <v-card class="mb-6 my-6">
                                For the Imperial IPA style, the analysis shows that th importance of the different characteristics is
                                <span class="primary--text">
                                more evenly distributed.
                                </span>
                                <br><br>
                                While taste is still the most influential factor, aroma and palate are close seconds and should also be taken into consideration when developing a beer in this style.
                                <br>
                                This indicates that a well-rounded approach to producing a high-quality Imperial IPA, with a focus on all aspects of the beer including taste, aroma, and palate, may be necessary for success in this market.
                            </v-card>
                        </v-col>
                    </v-row>
                </v-card-text>
            </v-card>
        </v-row>

        </v-container>
        </v-card>

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

        <v-card>
            <v-card-text>
                Based on the analysis of the most popular beers in Virginia, it appears that
                <span class="primary--text">
                taste is the most influential factor
                </span>
                for both the India Pale Ale (IPA) and Imperial IPA styles.

                <br><br>
                For the
                <strong> India Pale Ale (IPA) style, </strong>
                taste is the primary characteristic that sets the leading beers apart from their competitors.
                <br><br>
                For the
                <strong> Imperial IPA style, </strong> the importance of the different characteristics is more evenly distributed, with taste, aroma, and palate all being important factors.
                <br><br>

                <span class="text-subtitle-2">
                💡 Given these findings, we would advise our client to consider developing two beers – one regular IPA and one Imperial IPA – that prioritize these characteristics in their development.
                <br>
                This could involve focusing on producing a beer with a particularly high-rated taste, as well as ensuring that the aroma and palate are well-balanced and appealing to consumers.
                <br><br>
                By targeting these key aspects of the beer, our client can position themselves for success in the Virginia market and potentially surpass their competitors.
                </span>
            </v-card-text>

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
