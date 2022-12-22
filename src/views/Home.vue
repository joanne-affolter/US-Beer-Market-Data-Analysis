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
          <h1 class="font-weight-medium mb-5">
            teAmDreAm
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
          md="10"
          class="mx-auto"
        >
          <div class="pricing-trial-content d-flex justify-space-between flex-column flex-md-row">
            <div class="text-center text-md-left mt-7">
              <p class="text-2xl font-weight-medium primary--text mb-2">
                Our mission
              </p>
              <p>
                Our client, Sam Smith, recently graduated from college in Massachusetts and is interested in starting a brewery.
              </p>
              <p>
                He has noticed that local breweries are now trendy and wants to create a local vibe for his beer. He has already taken the first steps towards this goal by creating some sample beers and seeking feedback from his family and friends.
              </p>
              <p>
                However, he has received differing opinions on the quality and potential success of his brews, leaving him unsure of how to move forward. Seeking a more objective perspective, Sam has decided to turn to our consulting service for guidance.
              </p>
            </div>

            <!-- images -->
            <v-img
              contain
              max-width="100"
              src="@/assets/images/3d-characters/pose-fs-9.png"
              class="pricing-trial-img mx-auto"
              alt="svg img"
            />
            <!--/ images -->
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
          size="128"
        >
        <img
        src="@/assets/images/beer_advocate.png"
        >
        </v-avatar>
        </v-col>
        <v-avatar
          color="primary"
          size="128"
        >
        <img
        src="@/assets/images/rate_beer.png"
        >
        </v-avatar>
        <v-col cols="6" sm="6">

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
