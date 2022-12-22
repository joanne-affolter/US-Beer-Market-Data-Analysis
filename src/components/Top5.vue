<template>
    <v-card class="greeting-card my-6">
      <v-row class="ma-0 pa-0">
        <v-col cols="12">
          <v-card-title class="text-no-wrap pt-1 ps-2">
            <span class="primary--text">Average rating</span>
          </v-card-title>
          <v-card-subtitle class="text-no-wrap ps-2">
            for the 5 most similar beers
          </v-card-subtitle>
          <v-card-text class="d-flex align-center mt-2 pb-2 ps-2">
            <v-container>
              <v-row>
                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold warning--text mb-2">
                        Average over all ratings in Virginia
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        3.261/5
                    </p>
                  </div>
                </v-col>

                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold primary--text mb-2">
                        Williamsburg Irish Stout
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        2.8/5
                    </p>
                  </div>
                </v-col>

                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold primary--text mb-2">
                        Williamsburg Colonial Mild
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        2.5/5
                    </p>
                  </div>
                </v-col>

                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold primary--text mb-2">
                        Founders India Pale Ale
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        2.33/5
                    </p>
                  </div>
                </v-col>

                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold primary--text mb-2">
                        Blue & Gray Chocolate Raspberry Stout
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        2.58/5
                    </p>
                  </div>
                </v-col>

                <v-col cols="2" sm="2">
                  <div>
                    <p class="text-l font-weight-semibold primary--text mb-2">
                        Blue & Gray Bormans Belgian Ale
                    </p>
                    <p class="text-m font-weight-semibold mb-2">
                        2.5/5
                    </p>
                  </div>
                </v-col>

              </v-row>

              <v-row>
                    However, we can see that beers similar to our client's are not very well rated in general. Indeed, their average rating is lower than the average taken over all the beers rated in Virginia.
                    <br><br>
                    <div class='primary--text text-subtitle-2'>
                        💡 Our client must therefore offer other products in order to reach customers.
                    </div>
              </v-row>
            </v-container>
          </v-card-text>

        </v-col>


      </v-row>
    </v-card>
  </template>
