<template>
  <v-data-table
    :headers="headers"
    :items="results"
    :items-per-page="5"
    :item-class= "row_classes"
    class="elevation-1"
  >
  <template v-slot:item.calories="{ item }">
      <v-chip
        :color="getColor(item.name)"
        dark
      >
        {{ item.name }}
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
        { text: 'Number of users', value: 'nb' },
        { text: 'Number of breweries', value: 'nb2' },
        { text: 'Nb_users/Nb_breweries', value: 'rat' },
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
    getColor(state) {
      if (state == 'Massachusetts') return 'green'
      else if (state == Ohio) return 'green'
      else return 'orange'
    },
  },
}
</script>
