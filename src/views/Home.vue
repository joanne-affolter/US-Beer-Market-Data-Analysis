<template>
  <v-card
    id="pricing-plan"
    class="text-center py-sm-15 py-5"
  >
    <v-card-text>
      <v-row>
        <v-col
          cols="12"
          md="6"
          sm="8"
          class="mx-auto"
        >
          <h1 class="font-weight-medium mb-5 primary--text">
            About us
          </h1>
          <p class="mb-3">
            We are a consulting firm that specializes in helping breweries succeed through the use of data analytics. Our team has expertise in the brewery industry and utilizes a wide range of data sources to provide our clients with informed and strategic advice.
          </p>
        </v-col>
      </v-row>
    </v-card-text>

    <v-card-text class="pricing-free-trial my-16">
      <v-row>
        <v-col
          cols="12"
          md="12"
          class="mx-auto"
        >
          <div class="pricing-trial-content d-flex justify-space-between flex-column flex-md-row">
            <div class="text-center text-md-left mt-7">
              <p class="text-2xl font-weight-medium primary--text mb-2">
                Our mission
              </p>
              <br>
              <p class="mb-3">
                Our client, Sam Smith, recently graduated from college in Massachusetts and is interested in starting a brewery.
                He has noticed that local breweries are now trendy and wants to create a local vibe for his beer. He has already taken the first steps towards this goal by creating some sample beers and seeking feedback from his family and friends.
              </p>
              <p>
                However, he has received differing opinions on the quality and potential success of his brews, leaving him unsure of how to move forward. Seeking a more objective perspective, Sam has decided to turn to our consulting service for guidance.
              </p>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-card-text>
    <!--/ pricing free trial -->

    <v-card-text>
      <v-row align="center" justify="center">
        <v-col cols="6" sm="6">
          <v-avatar
            color="primary"
            size="100"
          >
          <img
          src="@/assets/images/beer_advocate.png"
          >
          </v-avatar>
        </v-col>
        <v-col cols="6" sm="6">
          <v-avatar
            color="primary"
            size="100"
          >
          <img
          src="@/assets/images/rate_beer.png"
          >
        </v-avatar>
        </v-col>
      </v-row>
    </v-card-text>

    <v-card-text class="my-16">
      <v-row>
        <v-col
          cols="12"
          md="8"
          sm="8"
          class="mx-auto"
        >
          <h1 class="font-weight-medium mb-5 primary--text">
            To help Sam create a successful brewery, we will follow a few steps.          </h1>
        </v-col>
      </v-row>
    </v-card-text>

    <v-card-text class="my-8">
      <v-row align="center" justify="center">
        <v-col cols="4" sm="4">
          <v-img src="@/assets/images/home1.jpg"></v-img>     </v-col>
        <v-col cols="8" sm="8">
          First, we will conduct a general market research on the beer industry in the United States. This will involve examining data on where consumers come from (by state), the evolution of the number of breweries over time, and trends in consumer behavior.
        </v-col>
      </v-row>
    </v-card-text>

    <v-card-text class="my-8">
      <v-row align="center" justify="center">
        <v-col cols="4" sm="4">
          <v-img src="@/assets/images/home2.jpg"></v-img>     </v-col>
        <v-col cols="8" sm="8">
          Once we have a good understanding of the overall market, we will focus on identifying the most promising states for Sam's brewery to operate in.
          <br><br>
          We will consider factors such as the size of the market, the level of competition, and the popularity of local breweries in each state. Our goal is to identify states that have a large market share, low competition, and a strong preference for local breweries.
        </v-col>
      </v-row>
    </v-card-text>

    <v-card-text class="my-8">
      <v-row align="center" justify="center">
        <v-col cols="4" sm="4">
          <v-img src="@/assets/images/home3.jpg"></v-img>     </v-col>
        <v-col cols="8" sm="8">
          After identifying a few states that meet these criteria, we will select one of them to focus on in more depth. We will examine the breweries and stats in this state to understand the competition and identify opportunities for Sam's brewery to stand out and succeed.
          <br><br>
          At this stage, we will also consider the feedback Sam has received from his family on his sample beers. We will use the business intelligence we have gathered thus far to evaluate this feedback and make recommendations for improvements to Sam's products. We may also suggest new products that we believe have the potential to perform well in the chosen state and fit with Sam's goal of creating a local vibe for his beer. Our goal is to help Sam create a successful brewery that meets the needs and preferences of local beer drinkers.
        </v-col>
      </v-row>
    </v-card-text>

  </v-card>
</template>

<script>
import { mdiCheckboxBlankCircleOutline } from '@mdi/js'
import { ref } from '@vue/composition-api'

export default {
  setup() {
    const status = ref(false)
    const pricingAccordion = ref(0)

    const pricing = {
      basicPlan: {
        title: 'Basic',
        monthlyPrice: 0,
        currentPlan: true,
        popularPlan: false,
        subtitle: 'A simple start for everyone',
        imgSrc: require('@/assets/images/misc/pricing-tree-1.png'),
        yearlyPlan: {
          perMonth: 0,
          totalAnnual: 0,
        },
        planBenefits: [
          '100 responses a month',
          'Unlimited forms and surveys',
          'Unlimited fields',
          'Basic form creation tools',
          'Up to 2 subdomains',
        ],
      },
      standardPlan: {
        monthlyPrice: 49,
        title: 'Standard',
        popularPlan: true,
        currentPlan: false,
        subtitle: 'For small to medium businesses',
        imgSrc: require('@/assets/images/misc/pricing-tree-2.png'),
        yearlyPlan: {
          perMonth: 40,
          totalAnnual: 480,
        },
        planBenefits: [
          'Unlimited responses',
          'Unlimited forms and surveys',
          'Instagram profile page',
          'Google Docs integration',
          'Custom “Thank you” page',
        ],
      },
      enterprisePlan: {
        monthlyPrice: 99,
        popularPlan: false,
        currentPlan: false,
        title: 'Enterprise',
        subtitle: 'Solution for big organizations',
        imgSrc: require('@/assets/images/misc/pricing-tree-3.png'),
        yearlyPlan: {
          perMonth: 80,
          totalAnnual: 960,
        },
        planBenefits: [
          'PayPal payments',
          'Logic Jumps',
          'File upload with 5GB storage',
          'Custom domain support',
          'Stripe integration',
        ],
      },
    }

    const faqsList = [
      {
        title: 'General settings',
        desc: 'Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.',
      },
      {
        title: 'Users',
        desc: 'Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.',
      },
      {
        title: 'Personal data',
        desc: 'Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.',
      },
      {
        title: 'Advanced settings',
        desc: 'Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.',
      },
    ]

    return {
      status,
      pricing,
      faqsList,
      pricingAccordion,
      icons: {
        mdiCheckboxBlankCircleOutline,
      },
    }
  },
}
</script>

<style lang="scss" >
@import '@core/preset/preset/mixins';
@import '@core/preset/preset/variables';

#pricing-plan {
  .popular {
    border-color: rgba(145, 85, 253, 0.3);
  }

  .pricing-free-trial {
    background-color: rgba(145, 85, 253, 0.04);
    position: relative;
    height: 14.625rem;
    .pricing-trial-img {
      position: relative;
      top: -3.5rem;
      right: 0;
    }
  }
  .pricing-accordion {
    .v-expansion-panels {
      .v-expansion-panel {
        box-shadow: none !important;
        margin-bottom: -1px;
        &::before {
          box-shadow: none;
        }
      }
    }
  }
}

@media (max-width: 960px) {
  #pricing-plan {
    .pricing-free-trial {
      height: auto;
      .pricing-trial-img {
        bottom: -1.2rem;
        top: unset;
      }
    }
  }
}

@include theme--child(pricing-accordion) using ($material) {
  .v-expansion-panels {
    .v-expansion-panel {
      border: 1px solid map-deep-get($material, 'dividers');
    }
  }
}
</style>
