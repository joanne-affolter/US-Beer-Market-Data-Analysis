<template>
    <div>
        <!--Title with image-->
        <v-card class="mb-6" color="primary">
            <v-img
                height="200"
                width="100%"
                src="@/assets/images/materio_img/mac_pc.png"
            ></v-img>

            <v-card-text class="d-flex align-center mt-5 text-h5 white--text font-weight-black">
                Market analysis
            </v-card-text>
        </v-card>

        <!--Introduction-->
        <v-card class="mb-6">
        <v-card-text>
            In this second part, we will determine who are the potential competitors of our client
            and in which state our client should locate its brewery.
        </v-card-text>
        </v-card>

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

    </div>
</template>

<script>
</script>
