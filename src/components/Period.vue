<template>
  <div>
  <v-container>
    <v-row>
      <v-col>
        <v-card>
          <v-card-title>
            <span class='text-subtitle-2 font-weight-bold primary--text'>
              Average number of users per year
            </span>
          </v-card-title>
          <v-card-text>
            <v-row>

              <v-col>
                <v-card>
                  <v-card-title>
                    <span class='font-weight-bold'>
                      2007 - 2011
                    </span>
                  </v-card-title>

                  <v-card-text class="pb-3 pt-5">
                    <!-- List -->
                    <v-list two-line subheader>
                      <!-- List Item: BA -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg success--text justify-center"
                                size="30"
                                rounded
                              >
                                <v-img src="@/assets/images/beer_advocate.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  32 003
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                      <!-- List Item: RB -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg primary--text justify-center"
                                size="30"
                                rounded
                              >
                              <v-img src="@/assets/images/rate_beer.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  24 209
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                    </v-list>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col>
                <v-card>
                  <v-card-title>
                    <span class='font-weight-bold'>
                      2011 - 2015
                    </span>
                  </v-card-title>

                  <v-card-text class="pb-3 pt-5">
                    <!-- List -->
                    <v-list two-line subheader>
                      <!-- List Item: BA -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg success--text justify-center"
                                size="30"
                                rounded
                              >
                                <v-img src="@/assets/images/beer_advocate.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  107 713
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                      <!-- List Item: RB -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg primary--text justify-center"
                                size="30"
                                rounded
                              >
                                <v-img src="@/assets/images/rate_beer.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  43 798
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                    </v-list>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col>
                <v-card>
                  <v-card-title>
                    <span class='font-weight-bold'>
                      2015 - 2017
                    </span>
                  </v-card-title>

                  <v-card-text class="pb-3 pt-5">
                    <!-- List -->
                    <v-list two-line subheader>
                      <!-- List Item: BA -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg success--text justify-center"
                                size="30"
                                rounded
                              >
                                <v-img src="@/assets/images/beer_advocate.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  107 713
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                      <!-- List Item: RB -->
                      <v-list-item class="pa-0">
                              <v-list-item-avatar
                                class="v-avatar-light-bg primary--text justify-center"
                                size="30"
                                rounded
                              >
                                <v-img src="@/assets/images/rate_beer.png"></v-img>
                              </v-list-item-avatar>
                              <v-list-item-content>
                                <v-list-item-title class="font-weight-semibold">
                                  17 862
                                </v-list-item-title>
                              </v-list-item-content>
                      </v-list-item>
                    </v-list>
                  </v-card-text>
                </v-card>
              </v-col>

            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({}),
}
</script>
