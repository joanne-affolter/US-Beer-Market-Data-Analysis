<template>
    <v-data-table
      :headers="headers"
      :items="results"
      :items-per-page="5"
      :item-class= "row_classes"
      class="elevation-1"
    >
    <template v-slot:item.state="{ item }">
        <v-chip
          :color="getColor(item.nb)"
          dark
        >
          {{ item.state }}
        </v-chip>
    </template>


    </v-data-table>
  </template>


  <script>
export default {
  data() {
    return {
      headers: [
        { text: 'State', value: 'state' },
        { text: 'nb_ratings/nb_users', value: 'nb' },
        { text: 'avg_rating_per_user', value: 'nb2' },
      ],
      results: [
        {
          state: 'Idaho',
          nb: 76.7,
          nb2: 239,
        },
        {
          state: 'Nevada',
          nb: 31.9,
          nb2: 160,
        },
        {
          state: 'Colorado',
          nb: 30.2,
          nb2: 133,
        },
        {
          state: 'Washington',
          nb: 28.9,
          nb2: 126,
        },
        {
          state: 'Arizona',
          nb: 27.3,
          nb2: 110,
        },
        {
          state: 'Tennessee',
          nb: 25.6,
          nb2: 142,
        },
        {
          state: 'Utah',
          nb: 25.3,
          nb2: 102,
        },
        {
          state: 'Minnesota',
          nb: 25.3,
          nb2: 127,
        },
        {
          state: 'Wisconsin',
          nb: 23.6,
          nb2: 93,
        },
      ],
    }
  },
  methods: {
    getColor(nb) {
      if (nb == 7332) return 'success'
      else if (nb == 5934) return 'success'
      else return 'warning'
    },
  },
}
</script>
