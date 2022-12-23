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
              Results of our analysis
            </h1>
            <p class="mb-3 text-subtitle-1">
                Our client has decided to open a local brewery in the US. Analyzing the beer market with data collected on RateBeer and BeerAdvocate websites brings out evidence on where to implement his new business and what to sell in order to maximize its success.
            </p>
          </v-col>
        </v-row>
      </v-card-text>

      <v-card class="mb-6" color="primary">
      <v-img
        height="300"
        width="100%"
        src="@/assets/images/bil2.jpg"
      ></v-img>
        </v-card>

      <v-card-text class="my-8">
        <v-row align="center" justify="center">
          <v-col cols="10" sm="10">
            First of all, we want to warn our client about the competitiveness of the beer market. We discovered that many new breweries only receive ratings during one year.  Consequently it is difficult to ensure long-lasting success for Sam’s brewery. Nevertheless, we perform an in-depth analysis of the market to give Sam Smith the tools to create a sustainable activity.
            <br><br>
            The complete analysis of all states of America has shown that Virginia stands out to be THE place to start a brewery. In fact, recently the number of users in Virginia has drastically increased which implies that new consumers are entering the market. And Virginians are more and more getting into local beers. Those new and local oriented customers will be thrilled to discover a new trendy brewery. Furthermore, even though there are many competitors none of them dominate the market and there are fewer breweries focused on local consumers than in other states. So Sam’s brewery will be easily settled in this environment.
            <br><br>
            The in-depth analysis of Virginia’s customers' taste has shown that the beer that Sam wanted to commercialize is not the most accurate, indeed he would be wiser to concentrate on creating beers with taste because it has been shown to be the characteristic which has the most impacts on users in Virginia. Those beers would be an IPA or Imperial IPA due to their high popularity in that state. In addition, we have found that the main appealing characteristic of IPA and Imperial IPA beers is taste which should be the aspect on which to focus on to succeed in the beer market. So Sam’s brewery beers should trend toward tasty regular and Imperial IPA to launch a thriving business.
          </v-col>
        </v-row>
      </v-card-text>

      <v-card class="mb-6" color="primary">
      <v-img
        height="300"
        width="100%"
        src="@/assets/images/bil1.jpg"
      ></v-img>
        </v-card>
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
