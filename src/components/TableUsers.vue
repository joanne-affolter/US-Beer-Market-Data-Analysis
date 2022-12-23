<template>
  <v-data-table
    :headers="headers"
    :items="results"
    :items-per-page="9"
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
        { text: 'nb_users', value: 'nb' },
        { text: 'nb_breweries', value: 'nb2' },
        { text: 'nb_users/nb_breweries', value: 'rat' },
      ],
      results: [
        {
          state: 'California',
          nb: 14442,
          nb2: 1796,
          rat: 8.0,
        },
        {
          state: 'Pennsylvania',
          nb: 10321,
          nb2: 626,
          rat: 16.5,
        },
        {
          state: 'New York',
          nb: 8784,
          nb2: 790,
          rat: 11.1,
        },
        {
          state: 'Illinois',
          nb: 8272,
          nb2: 504,
          rat: 16.4,
        },
        {
          state: 'Texas',
          nb: 7316,
          nb2: 518,
          rat: 14.1,
        },
        {
          state: 'Florida',
          nb: 5873,
          nb2: 532,
          rat: 11.0,
        },
        {
          state: 'Michigan',
          nb: 5354,
          nb2: 637,
          rat: 8.4,
        },
        {
          state: 'Massachusetts',
          nb: 7332,
          nb2: 333,
          rat: 22.0,
        },
        {
          state: 'Ohio',
          nb: 5934,
          nb2: 456,
          rat: 13.0,
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
