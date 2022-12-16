<template>
    <div>
        <!--Title with image-->
        <v-card class="mb-6" color="primary">
            <v-img
                height="200"
                width="100%"
                src="@/assets/images/materio_img/mac-pc.png"
            ></v-img>

            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                Market analysis
                <span class="text-h6">
                    In this second part, we will determine who are the potential competitors of our client
                    and in which state he should locate its brewery.
                </span>
            </v-card-text>

        </v-card>

        <!-- Specifications -->
        <v-card>
            <v-card-title class="align-start">
                Let's note we were given the following specifications :
                <v-spacer></v-spacer>
            </v-card-title>

            <v-card-text>
                <v-timeline dense class="timeline-custom-dense timeline-custom-dots">

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        Passionate about beer, he wants to be as close as possible to his customers and therefore wants to reach a local clientele in the state where he will set up his brewery.
                    </h4>
                    </div>
                </v-timeline-item>

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        He is not able to produce more than 30 beers.
                    </h4>
                    </div>
                </v-timeline-item>

                <v-timeline-item small color="primary">
                    <div class="d-flex justify-space-between align-center flex-wrap">
                    <h4 class="font-weight-semibold me-1">
                        He is open to all states to set up his brewery.
                    </h4>
                    </div>
                </v-timeline-item>

                </v-timeline>
            </v-card-text>
        </v-card>

        <!--I. Title with avatar-->
        <v-card class="mb-6" color="primary">
        <v-container>
            <v-row>

            <v-col cols="8" sm="6">
                <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                    Where should you open you brewery ?
                </v-card-text>
            </v-col>

            <v-col cols="4" sm="6">
                <v-img
                width="121"
                src="@/assets/images/3d-characters/pose-2.png"
                class="gamification-john-pose-2"
                ></v-img>
            </v-col>

            </v-row>
        </v-container>
        </v-card>

        <!-- Introduction -->
            <!--Introduction-->
            <v-card class="mb-6">
                <v-card-text>
                    In order to determine which states our client should open its brewery in, we will chose the top 3 states based on thses criterias :
                </v-card-text>
                <v-actions>
                    <v-row align='center' justify="center">

                        <v-col>
                            <v-btn elevation="13" rounded text x-large color="#F3E5F5">
                                A large market share to reach with a lot of potential clients
                            </v-btn>
                        </v-col>

                        <v-col>
                            <v-btn elevation="13" rounded text x-large color="#E1BEE7">
                                Consumers who like local beers
                            </v-btn>
                        </v-col>

                        <v-col>
                            <v-btn color='#CE93D8' elevation="13" rounded text x-large>
                                Beer lovers who make a lot of ratings
                            </v-btn>
                        </v-col>

                    </v-row>
                </v-actions>
            </v-card>





    </div>
</template>

<script>
</script>
