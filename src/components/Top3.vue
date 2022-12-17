<template>
  <v-card class="greeting-card">
    <v-row class="ma-0 pa-0">
      <v-col cols="8">
        <v-card-title class="text-no-wrap pt-1 ps-2">
          <span>The </span>
          <span class="primary--text"> top 3 states</span>
        </v-card-title>
        <v-card-subtitle class="text-no-wrap ps-2">
          for our client's brewery location
        </v-card-subtitle>
        <v-card-text class="d-flex align-center mt-2 pb-2 ps-2">
          <v-container>
            <v-row>
              <v-col cols=4>
                <div>
                  <p class="text-xl font-weight-semibold primary--text mb-2">
                    Washington
                  </p>
                  <p class="text-l font-weight-semibold mb-2">
                    With the highest score and a low number of competitors
                  </p>
                </div>
              </v-col>

              <v-col cols=4>
                <div>
                  <p class="text-xl font-weight-semibold primary--text mb-2">
                    Virginia
                  </p>
                  <p class="text-l font-weight-semibold mb-2">
                    With the highest score, many competitors but a strong community of beer lovers.
                  </p>
                </div>
              </v-col>

              <v-col cols=4>
                <div>
                  <p class="text-xl font-weight-semibold primary--text mb-2">
                    Massachusetts
                  </p>
                  <p class="text-l font-weight-semibold mb-2">
                    With the second best score and a low number of competitors
                  </p>
                </div>
              </v-col>
            </v-row>
          </v-container>
        </v-card-text>

      </v-col>

      <v-col cols="4">

        <v-img
          contain
          height="130"
          max-width="83"
          class="greeting-card-trophy"
          src="@/assets/images/misc/trophy.png"
        ></v-img>
      </v-col>
    </v-row>
  </v-card>
</template>

<style lang="scss" scoped>
.greeting-card {
  position: relative;
  .greeting-card-bg {
    position: absolute;
    bottom: 0;
    right: 0;
  }
  .greeting-card-trophy {
    position: absolute;
    bottom: 10%;
    right: 8%;
  }
}
// rtl
.v-application {
  &.v-application--is-rtl {
    .greeting-card-bg {
      right: initial;
      left: 0;
      transform: rotateY(180deg);
    }
    .greeting-card-trophy {
      left: 8%;
      right: initial;
    }
  }
}
</style>
