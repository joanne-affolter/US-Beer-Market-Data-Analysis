<template>
<div>
    <!--Title with image-->
    <v-card class="mb-6" color="primary">
        <v-img
            height="200"
            width="100%"
            src="@/assets/images/4top.jpg"
        ></v-img>

        <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                Leading breweries in the 3 recommended states
        </v-card-text>
    </v-card>

    <!-- Intro -->
    <v-card class="mb-6 my-8">
        <v-container>
            <v-row class="ma-0 pa-0">
              <v-col cols="9" sm="9">
                <v-card-text class="text-subtitle-2 font-weight-bold">
                    To detect potential competitors of our client, we will find which breweries...
                </v-card-text>
                <v-card-actions>
                    <v-container>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary" class="my-4">
                                are the most popular with the highest number of ratings
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary" class="my-4">
                                have been established in the area for a long time with the longest period since the first rating
                            </v-btn>
                        </v-row>
                        <v-spacer></v-spacer>
                        <v-spacer></v-spacer>
                        <v-row>
                            <v-btn elevation="13" rounded text large dark color="primary" class="my-4">
                                are local with the highest percentage of ratings within the state
                            </v-btn>
                        </v-row>
                    </v-container>
                </v-card-actions>
              </v-col>
            </v-row>
            <v-row>
                <v-card>
                    <v-card-text>
                        By examining these different criteria, we will assign scores to each brewery and then determine which ones are the strongest on the market and therefore which breweries represent the biggest competitors of our client.
                        <br><br>In parallel, we will compare the 3 states to finally retain one for the next part of our work.
                    </v-card-text>
                </v-card>
            </v-row>
        </v-container>
    </v-card>

    <!-- -->
    <v-card class="mb-6" color="primary" >
        <v-container>
            <v-row>
                <v-col cols="8" sm="6">
                    <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                        <span class="text-h5 font-weight-black ">
                        Highest number of ratings
                        </span>
                        <span class="text-subtitle-2">
                            We'll start by determining which breweries are the most popular in each state by determining the total number of ratings per brewery.
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
