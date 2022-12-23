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
                Our client, Sam Smith, has decided to open a local brewery in the United States and has enlisted our consulting services to help him identify the best location and products for his business.             </p>
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
            Using data from RateBeer and BeerAdvocate, we have analyzed the beer market and determined that Virginia is the most promising state for Sam's brewery. Virginia has a rapidly growing number of users, a strong preference for local beers, and evenly distributed competition levels, making it an ideal location for Sam's business.
            <br><br>
            However, we want to caution Sam about the competitiveness of the beer market. Many new breweries only receive ratings for a short period of time, which can make it challenging to achieve long-term success. Therefore, we have performed an in-depth market analysis to provide Sam with the tools he needs to create a sustainable business.          </v-col>
            <br><br>
            We compared the reviews that Sam gathered on his first brews with the reviews of Virginian beers to identify specific competitors and analyze their characteristics. We found that the closest competitors significantly outperformed Sam's brews in terms of taste, which we determined to be the most important aspect based on feature importance analysis. While Sam's beer has a decent appearance and palate, it won’t be enough to compete with his competitors and establish a foothold in the Virginian beer market. As a result, we suggested new flagship products that incorporate the best features of the most successful beers in Virginia.
            <br><br>
            Our analysis of Virginia's consumer preferences shows that Sam should focus on creating beers with strong taste, particularly IPAs and Imperial IPAs, which are particularly popular in that state. These beers are known for their taste, which is the most important factor for Virginia's beer drinkers. By concentrating on creating tasty IPAs and Imperial IPAs, Sam's brewery can stand out in the crowded beer market and succeed.
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
